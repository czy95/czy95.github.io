---
layout: post
---
### VR/AR Related Papers
* [Scenario-Based Construction Safety Training Platform Using Virtual Reality](https://www.iaarc.org/publications/fulltext/ISARC_2020_Paper_379.pdf)
  - 现象: VR，AR用于安全培训
  - 应用场景：前期阶段，模拟施工阶段，工人，
  - 特性： 
    1. 现存VR平台，缺乏良好框架方法，无法普及
    2. VR模拟大多关注方向风险，很少关注减轻风险
    3. 构建VR安全训练平台的费用高
  - Method：
    1. Decision-Making Accident Scenario(DMAS)模型，高度整合
    2. 设备：Unity and Google VR SDK， google cardboard, headphones, smartphone-based VR platform, Revit, Maya(**介绍了为什么要用**）
      - 介绍了Unity，
    3. 如果有操作错误会有意外报警。
    4. 具体步骤：
      1. RIF+ARP-risk identification framework. 分类现场风险,包含类别，原因，和预警措施3部分（ARP)
        - OSHA指南+实地考察缩减范围
      2. Accidental situations(As) + Possible Accidents(PA) -by site visit
      3. 依据As和VR找出A,依据RIF得到P.(CP/IP)
      4. 在VR中建模
  - Evaluation：
    - parameters: 1. identifying risks correctly. 2. suggesting corresponding precautions
    - **Feeback Questionaire**
  - Results：
    - 识别结果不好，证明VR的重要性。。
  - Others: 
    - Revit was not a non-uniform rational B-spline (NURBS) modeler, which generally helped in manipulating 3D curves and surfaces of any object, it couldn't be used for creating these models
  - `My thoughts： 结果不好，会不会有其他的原因。逻辑`
  
* [An Assistive Interface of a Teleoperation System of an Excavator by Overlapping the Predicted Position of the Arm](https://www.iaarc.org/publications/fulltext/ISARC_2020_Paper_97.pdf)
  - 现象：用遥控液压挖掘机在灾后进行快速安全施工
  - 应用场景：灾后重建，驾驶员
  - 特性：
    1. communication delay存在，操作时间长
  - Method: 降低操作时长
    1. 用一阶延迟方程预测模拟位置（提前预估），然后让计算3种情况下的运行时间
    2. 设备：unity3D,A joystick (Logitech Extreme 3D Pro)
  - Results:
    1. with delay + predition 比现实模拟（without delay and predition)相比差不多，可能是因为重叠导致。（*改进策略，一定距离不显示*）
    2. 比without prediction好， Fisher's LSD（统计测量）
* [Constructible Design for Off-site Prefabricated Structures in Industrial Environments: Review of Mixed Reality Applications](https://www.iaarc.org/publications/fulltext/ISARC_2020_Paper_127.pdf)
  - 现象：棕地开发
  - 应用场景：施工，工人
  - 特性： 
    1. 棕地开发复杂（场地设施权限，需要探测地下设备结构，安全，计划）.constructability不行
    2. 预制是定制的，意味组装阶段不能改，constructability不行
  - Methods（最好要和特性一一对应）: MR叠加到现实,提高constructability, optimize stragety
  - Others：
    - 提到了MR的第4个特性，storage
    - 提到了AR对建设活动有作用（他人，包括自己也证实了）。Shin et al.identified work tasks as well as construction activities that can benefit from Augmented Reality based on technology suitability [6].
      1. 布置和定位
      2. 开挖
      3. 策划
  - `没有论证。。纯理论文章`
    
* [测试链接SCI-HUB功能](https://sci-hub.do/10.1061/(asce)co.1943-7862.0001749)

