# Schéma de fichier
- Contrôle de Pendule Inversé basé sur MPC ---- Une Sorte de Contrôle Optimal.pdf
- code
	- Cart_Pole_MPC_doc.slx
	- Inv_Pendulum_modeling.mlx
	- Inverted_Pendulum.mlx
- README.md

# Compilation
Si vous souhaitez exécuter cette simulation, exécutez le script Inverted_Pendulum.mlx en premier, puis compilez et exécutez simulink.

# Copie du code
- Les matrices quadratiques sont calculées
```MATLAB
[m1, n1] = size(model.A);
[n1, n_in] = size(model.B);

%% calculate M
n = m1 + n1;
h(1:m1,:) = eye(m1);
E(1:m1,:) = eye(m1) * model.A;

for kk = 2 : param.Np
h((kk - 1) * m1 + 1 : kk * m1, :) = h((kk - 2) * m1 + 1 : (kk - 1) * m1,:) * model.A;
E((kk - 1) * m1 + 1 : kk * m1, :) = E((kk - 2) * m1 + 1 : (kk - 1) * m1, :) * model.A;
end

%% Calculate C
% first column of C
v = h * model.B;
F = zeros(param.Np * m1, param.Np * n_in);
F(:,1 : n_in) = v;

% Other columns of \Phi
for i = 2 : param.Np
F(:,(i-1) * n_in + 1 : i * n_in) = [zeros((i-1) * m1, n_in);v(1:(param.Np - i + 1) * m1, 1 : n_in)];
end

model.E = E; % M
model.F = F; % THETA
refs = repmat(ref,Np,1);
H = 2 * ((F.')*q*F + r);
g = (F.')*q*( E * states- refs );
```
- Calculer la matrice de poids

```MATLAB
% Q,R
model.Q = [10 0 0 0
0 40 0 0
0 0 1 0
0 0 0 1];
model.R = 0.0001;
model.q = [];
model.r = [];

for i = 1:param.Np
model.q = blkdiag(model.q, model.Q);
model.r = blkdiag(model.r, model.R);
end

  

model.ll = repmat(param.lower, param.Np, 1);
A = repmat(10,3,2)
model.uu = repmat(param.upper, param.Np, 1);
```
- Résolu par la méthode des points intérieurs
	Nous nous référons ici à certaines des façons dont l’IA est écrite.
```MATLAB
function res = interior_point_qp(H, f, A, b, x0, max_iter, tol, mu)

% Description des paramètres：
% H: Matrice des coefficients quadratiques
% f: Vecteur de coefficient linéaire
% A: Une matrice de coefficients contraints par les inégalités
% b: Le vecteur sur le côté droit de la contrainte d’inégalité
% x0: Vecteur de solution initiale
% max_iter: Nombre maximal d’itérations
% tol: Tolérance de convergence
% mu: Paramètre central
n = length(x0);
m = size(A, 1);

% initialisation
x = x0;
s = ones(m, 1);
lambda = ones(m, 1);
mu_k = mu * ones(m, 1);
iter = 0;

while iter < max_iter

% Calculer le décalage du centre
F = H * x + f - A' * lambda - s;

% Calculer la condition centrale
centering_condition = norm(F, Inf);
if centering_condition < tol
break;
end

% Construire une matrice de chemin central
KKT_matrix = [H, -A'; A, -diag(lambda) * diag(s)];
rhs = [-H * x - f; -A * x + b - mu_k .* s];

% Résoudre des systèmes linéaires
delta = KKT_matrix \ rhs;

% Mettre à jour les vecteurs et les multiplicateurs de solution
delta_x = delta(1:n);
delta_lambda = delta(n+1:end);
x = x + delta_x;
lambda = lambda + delta_lambda;
s = mu_k ./ lambda;
iter = iter + 1;
end

% fval = 0.5 * x' * H * x + f' * x;
res = x(1);
end
```