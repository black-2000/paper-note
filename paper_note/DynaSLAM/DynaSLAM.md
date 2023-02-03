# DS-SLAM: A Semantic Visual SLAM towards Dynamic Environmentsz
作者：Chao Yu, Zuxin Liu, Xin-Jun Liu, Fugui Xie, Yi Yang, Qi Wei, Qiao Fei

机构：清华大学、北航

2018年发表于IROS

主要内容提出了DS-SLAM，五线程并行：跟踪、语义分割、局部地图构建、回环检测、密集语义地图构建。采用语义分割和运动一致性检查的方法识别动态物体

所用数据集：TUM RGB-D dataset、real-world environment

## 现有方法的不足

- 现有框架不够鲁棒，不能适用于所有的环境之中，如高度动态或者恶劣环境之中。

- 地图模型通常是基于几何学的信息，如基于地标的地图和点云地图，所以它们并不提供对周围环境的任何高层次的理解。




识别动态物体的方法：1、光流法   耗时短，但精度差


## 整体结构

所用传感器：Kinect v2

建图与回环检测与ORB2相同

语义分割网络采用SegNet


摘用：1、However, some problems are still
not well solved, for example, how to tackle the moving objects in
the dynamic environments, how to make the robots truly
understand the surroundings and accomplish advanced tasks.

2、Images store a wealth of information and can be employed for other vision-based applications, like semantic segmentation and object detection.

3、According to [3], SLAM enters the robust-perception age and more research to achieve genuinely robust perception and navigation for autonomous robots is needed.

4、A basic assumption in most current SLAM approaches is that the environment is static. However, active objects like humans, exist in many real-world scenes. Therefore, most state-of-the-art approaches that initially designed for doing SLAM in static environments are not capable of handling severe dynamic scenarios. 
