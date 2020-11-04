## resource + idea + plan
### resource
- unity3d
  - [调整物体pivot ponits插件](https://learn.unity.com/tutorial/setting-pivot-points-in-the-pixyz-plugin?utm_source=learn_recommendation)
  - [unitylearn](https://learn.unity.com/)
    - **优先for deep learning**[unity HDRP](https://learn.unity.com/project/up-and-running-with-hdrp)
    - [unity VR](https://learn.unity.com/project/vr-beginner-the-escape-room)
    - [unity Reflect](https://learn.unity.com/course/getting-started-with-reflect?_ga=2.29603199.197386871.1603944811-1626180048.1602888992)
    - [unity ROS#](https://github.com/siemens/ros-sharp)
    - [unity ML-agents]
  - 之前可能有BIM导入unity材质丢失的问题，[通过3dmax中转或者C#好像可以解决](https://www.zhihu.com/question/265783552)。我下载的插件似乎就是C#写好能导入fbx的 or 外包。
  - https://www.cm-labs.com/vortex-studio/

- Robot
  - [2018年资料](https://zhuanlan.zhihu.com/p/32788790)
    1. 区别于机器人设计工具 solidworks， blender。具备物理引擎：Bullet, ODE,MuJoCo(商业引擎不开源）, unity3D用的是PhysX(nvidia,带N卡的gpu加速功能)。havok（专注CPU+多线程模拟，不免费）
      - [ICRA 2015对5种引擎进行了对比分析](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=7139807&tag=1)
    2. unity3D的物理引擎没有destruction，对于车辆只有车轮模拟，不开源（havok可以弥补）
    3. 仿真工具Gazebo, V-REP, Webot(商业）
      - gazebo, ROS的，支持bullet和ODE，和ROS兼容性好（很重要）。模型格式是基于XML的SDF（simulation description format).命令行，上限大
      - V-REP，bullet, ode,vortex(流体仿真），相比gazebo集成了很多常见模型，建模简单，兼容ROS
      - **Gazebo的优势在于与ROS完全兼容性、开源，而V-REP更为直观、方便使用，集成了更多的特性。**
      - [follow the line (ROS+V-REP)，SLAM，4年前。。](https://github.com/Nurgak/Virtual-Robot-Challenge)
    4. [四足机器人建模gazebo，slam,moveit](https://www.zhihu.com/column/c_1010846380042174464)
      - [四足站立](https://zhuanlan.zhihu.com/p/64321561)
    5. LZJ的turtlebot
- path planning
    1. [Autoware-AI](https://github.com/Autoware-AI/autoware.ai)
- Python
    - [if __name__ == "__main__"的作用](https://www.zhihu.com/question/49136398)
    - c# c++等都需要有程序入口（main 编译性语言），进行编译为二机制语言,python是脚本语言，逐行解释运行，没有统一入口，可以被直接运行或作为模块导入。两种情况下的顶层代码都会被运行。但是实际有些情况下的代码（尤其import的）是不想运行的。所以需要main
  
- 画图软件
  - originlab(gif)
- math
  - 最小二乘法和正太分布（高斯分布）为充要条件，联合概率，极大似然估计
    

  - machine learning
- [解释结构模型](http://www.huaxuejia.cn/ism/how_to_use_ism.php)

  
### idea

### plan

