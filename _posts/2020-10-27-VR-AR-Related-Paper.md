---
layout: post
---
现象：广泛存在、可循环、会反复出现。如绑扎钢筋失败。会涉及各阶段。
## ISARC-Meeting
### 1. [Scenario-Based Construction Safety Training Platform Using Virtual Reality](https://www.iaarc.org/publications/fulltext/ISARC_2020_Paper_379.pdf)
  - **现象: VR，AR用于安全培训**
  - 应用场景：前期阶段，模拟施工阶段，工人，
  - 特性： 
    1. 现存VR平台，缺乏良好框架方法，无法普及
    2. VR模拟大多关注方向风险，很少关注减轻风险
    3. 构建VR安全训练平台的费用高
  - Method：
    1. Decision-Making Accident Scenario(DMAS)模型，**高度整合, 而且关注了降低风险的操作**
    2. 设备：Unity and Google VR SDK， google cardboard, headphones, smartphone-based VR platform, Revit, Maya(**介绍了为什么要用**）
      - 介绍了Unity，
    3. 具体步骤：
      1. RIF+ARP-risk identification framework. 分类现场风险,包含类别，原因，和预警措施3部分（ARP)
        - OSHA指南+实地考察缩减范围
      2. 定义风险场景（便于识别后面风险）Accidental situations(As) + Possible Accidents(PA) -by site visit
      3. 依据As和VR找出A,依据RIF得到P.(CP/IP)（依靠场景，识别可能的风险，以及可能的改进方式）
  - Evaluation：VR unity评测
    - parameters: 1. identifying risks correctly. 2. suggesting corresponding precautions
    - **Feeback Questionaire**
    - 识别结果论证了风险很多，证明VR的重要性。。
  - Others useful: 
    - 说了revit建非建筑不规则模型的弱势。Revit was not a non-uniform rational B-spline (NURBS) modeler, which generally helped in manipulating 3D curves and surfaces of any object, it couldn't be used for creating these models
  - `My thoughts： 结果不好，会不会有其他的原因。比如模型不行，不够仿真。不过作者解释是从人员思想上来解释的`
  
### 2. [An Assistive Interface of a Teleoperation System of an Excavator by Overlapping the Predicted Position of the Arm](https://www.iaarc.org/publications/fulltext/ISARC_2020_Paper_97.pdf)
  - **现象：用遥控液压挖掘机在灾后进行快速安全施工**
  - 应用场景：灾后重建，驾驶员
  - 特性：
    1. communication delay存在，操作时间长
  - Method: 降低操作时长
    1. 用一阶延迟方程预测模拟位置（提前预估），然后让计算3种情况下的运行时间
    2. 设备：unity3D,A joystick (Logitech Extreme 3D Pro)
  - Results:
    1. with delay + predition 比现实模拟（without delay and predition)相比差不多，可能是因为重叠导致。（*改进策略，一定距离不显示*）
    2. 比without prediction好， Fisher's LSD（统计测量）
    
### 3. [Constructible Design for Off-site Prefabricated Structures in Industrial Environments: Review of Mixed Reality Applications](https://www.iaarc.org/publications/fulltext/ISARC_2020_Paper_127.pdf)
  -** 现象：棕地开发可建造性不行**
  - 应用场景：施工阶段，工人
  - 特性： 
    1. 棕地开发复杂（场地设施权限，需要探测地下设备结构，安全，计划）.constructability不行
    2. 预制是定制的，意味组装阶段不能改，constructability不行
  - Methods（最好要和特性一一对应）: 
    - MR叠加到现实,提高constructability, optimize stragety
    - 定性分析了layout & position, excavation, stategizing三个阶段。。（**没有论证**）
  - Others：
    - ***提到了MR的第4个特性，storage***
    - 提到了AR对建设活动有作用（他人，包括自己也证实了）。Shin et al.identified work tasks as well as construction activities that can benefit from Augmented Reality based on technology suitability [6].

### 4. [Five-dimensional Simulation of Bridge Engineering Based on BIM and VR](https://www.iaarc.org/publications/fulltext/ISARC_2020_Paper_14.pdf)
  - **应用场景: construction management。施工管理阶段。**
  - 特性：4D用的很多，但是cost不多。method本文做了5D，bridge的建造阶段（前期预制和后期排除）
  - x:用的Fuzor做的VR simulation/annimation
  
### 5. [A Construction Progress On-site Monitoring and Presentation System Based on The Integration of Augmented Reality and BIM](https://www.iaarc.org/publications/fulltext/ISARC_2020_Paper_41.pdf)
  - **现象：施工进度管理与决策还是不够**
  - 应用场景：施工阶段，管理人员的实时管理，可视化工具不行 **施工阶段变化最多且最容易出错**
  - 特性：
    - 大多不能real-time,
    - GPS等装置安装麻烦
    - 大多数研究关注是在户外（信号）和既有建筑。
  - method：
    - dynamic references + SLAM + BIM（phased),可以实现室内，real-time，免安装设备(wifi)等好处。**kevin是既有建筑用wifi footprint**
  - others:
    - 把模型分层存储，节约空间
    
### 6. Factors affecting the adoption of AR in AEC by [SLR-ISM](https://link.springer.com/article/10.1007/s10901-019-09674-y) or TAM(https://baike.baidu.com/item/%E6%8A%80%E6%9C%AF%E6%8E%A5%E5%8F%97%E6%A8%A1%E5%9E%8B/2184121?fr=aladdin)
TITLE ( "Mixed Reality"  OR  "MR"  OR  "Virtual Reality"  OR  "VR"  OR  "Augmented Reality"  OR  "AR" )  AND  TITLE ( "factors affecting"  OR  "barriers" ) 

