# Step 1
## Introduction
看上去像是为了使机器人获得杂耍般的运动性能。目前的足式机器人在运动性能上已经有了很大的进步，但是还是没有和真正的生物一样的灵活性。
- 要提高身体灵活性，基于模型控制的机器人会遇到算力上的问题。
- 控制器需要丝滑地合成不同的运动，或者连接不同的运动。
此前的工作对机动的开始状态和结束状态有着极高的要求。

轨迹 -》架构 -〉 机器人可执行指令

加速 Whole-body MPC
结合 RICCATI 控制器和whole body QP，使其结果满足约束
## Structure
- Related work
	-  MPC 
		- template MPC, 需要一个底层的控制器去产生全身控制指令。可能 MPC 给出的结果底层控制器发现是做不到的。
		- Whole-body MPC，计算量很大。现在优化到能用，但是高灵活性的还没有。
		- MHPC，综合以上两种。但是 model combine 的顺序会影响性能。
		- Contact-implicit MPC，数值求解上的问题和运算量。
	- MPC 数值优化，因为 MPC 控制很重要的成果因素就是如何解决背后的轨迹优化问题
		- 直接方法
		- DDP：有效的约束应对和 sensitivity to initial guess
	- WBC，为 MPC 计算可供机器人具体执行的指令
		- 将其看作一个 QP problem，就是一个二次型。non-trivial tuning.1. 任务权重是启发性的；2. tasks design uses 简化模型，跟问题中的全身动力学不连贯；3. 只保证短期稳定性
		- Riccati controller，结果不一定满足约束
		- VWBC：用了新的目标函数保证了长期稳定性，来自于 CAFE-MPC，同时让 Riccati controller 满足了约束？
	- RL，有进步但还比不上最优化结果
		- 鲁棒性有，精度不足
- Multiple-shooting Differential Dynamic Programming；多 phases，stated-based switching hybrid system；这是在为 CAFE- MPC做准备工作。
	- 多次打靶法，单 phase 系统
	- 多次打靶法，多 phase 系统
- Cascaded-Fidelity Model Predictive Control。一开始精细，起飞后粗糙
	- Whole-body plan formulation
	- tailing plan formulation
	- Connecting the two
	- Whole-body plan formulation 可根据足端触地情况继续进行细分
- Value-Based Whole Body WBC
	- Whole-body MPC 阶段，直接用 MPC 结果就好了；或者采用Riccati controller 优化每个 MPC 周期内的控制量，使其更丝滑。后果是控制指令可能不在约束范围内。
- Implementation Details
- Results
	- CAFE-MPC
	- Extend multiple-shooting iLQR to a class of hybrid system
	- VWBC
- Conclusion