# Introduction
足式机器人有步态概念，可能每时每刻足端与地面的接触状态都在发生变化。每一次变化都会相应的改变机器人的运动学方程。这给 MPC 带来了挑战。
目前仍旧缺少比较通用的控制器：
- 不需要特定应用简化模型的
- 不需要步态启发生成
- 不需要巨量参数调整

# Structure
- Related work
	- MPC
		- 当前 MPC 局限性，通常只适用于特定系统
	- Complementarity-Based Contact Dynamics
		- 使用LCP来模拟刚体动力学中的接触相互作用的经典方法
		- 隐式微分、内点法
		- LCP 用于规划
		- Mujoco
- Background(pre-work)
	- MPC
	- Complementarity-Based Contact Dynamics
	- Interior-Point Method
	- Implicit Differentiation
		- 求解解的敏感度
- CI-MPC
	- Time-varying Contact Dynamics
	- Fast Contact Dynamics
	- Gradients
	- Planning
	- Contact-height Heuristic
	- Algorithm
	- Heuristics
- Results
	- simulation
		- 提高频率如何证明对采样率的鲁棒性
		- 
	- hardware

# Result
- fast approximate contact dynamics
- Structure exploiting solver
- MPC framework

- Limitations
	- 模型中有 approximation，这在当前还好，但是如果加长预测周期不知道会带来什么影响。
	- 还有不同种的方法可供比较。软接触模型让轨迹跟踪求解器更容易收敛，并且让策略更容易找到新的步态。是否有需要建立严格的硬接触模型。
	- 轨迹生成方法收敛性很差，导致不太能用于在线计算
	- 可以尝试加入 Convex MPC 中那样的落点选择策略，有利于加速和增强可靠性。
	- 

# Questions
- What are heuristics
- LCP
- Pivoting method
- Implicit differentiation
- Interior-Point Method
- Collocation Method
- Complementarity-based Contact Dynamics
- 隐函数定理