# Step 1
## Introduction
MPC 控制在小型机器人上很有前途。但是受限于小型机器人的供能、算力等等问题，很难部署 MPC 算法。尽管现在已经有了给嵌入式系统开发的凸优化求解器，但还是不够好。
本文给出了为 MCU 定制的，不用求逆的，开源 C++ 实现的实时 MPC 优化求解器。
## Structure
- Introduction
- Background
	- LQR
	- Convex MPC
	- ADMM
- TinyMPC Solver
	-  LQR & ADMM for MPC
	- Pre-commutation
	- Penalty scaling
- Experiments
	- Microcontroller benchmark
	- 8 字型轨迹跟踪
	- 大偏离姿态稳定
	- 动态障碍躲避
- Conclusion & Future work
## Conclusion
- ADMM 处理状态和输入限制
- 充分利用 MPC 问题结构
- Insights from LQR
- 在 CrazyFlie 四旋翼无人机上测试。

# Step 2
有待仔细研究下 ADMM 是种什么方法。
And 研究一下 LQR
得复习一下拉格朗日乘子