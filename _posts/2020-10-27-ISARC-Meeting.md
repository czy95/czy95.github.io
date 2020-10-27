---
layout:post
---
### Related Papers
* [Scenario-Based Construction Safety Training Platform Using Virtual Reality](https://www.iaarc.org/publications/fulltext/ISARC_2020_Paper_379.pdf)
  - 现象: VR，AR用于安全培训
  - 应用场景：前期阶段，工人，
  - 特性： 
    1. 现存VR平台，缺乏良好框架方法，无法普及
    2. VR模拟大多关注方向风险，很少关注减轻风险
    3. 构建VR安全训练平台的费用高
  - Method：
    1. Decision-Making Accident Scenario(DMAS)模型，高度整合
    2. 设备：Unity and Google VR SDK， smartphone-based VR platform
  - Results：
  - `My thoughts`
  
* [An Assistive Interface of a Teleoperation System of an Excavator by Overlapping the Predicted Position of the Arm](https://www.iaarc.org/publications/fulltext/ISARC_2020_Paper_97.pdf)
  - 现象：用遥控液压挖掘机在灾后进行快速安全施工
  - 应用场景：灾后重建，驾驶员
  - 特性：
    1. communication delay存在
  - Method: 
    1. 用一阶延迟方程预测模拟位置（提前预估），然后让计算3种情况下的运行时间
    2. 设备：unity3D,A joystick (Logitech Extreme 3D Pro)
  - Results:
    1. with delay + predition 比现实模拟（without delay and predition)相比差不多，可能是因为重叠导致。（*改进策略，一定距离不显示*）
    2. 比without prediction好， Fisher's LSD（统计测量）
