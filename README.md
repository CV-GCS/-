# 沿江巡逻机器人系统
沿江巡逻机器人系统——实现ROS智能机器车的SLAM巡航、AI智能识别、警报提醒等功能。获得集创赛算能杯华南赛区二等奖。

【项目展示】
https://docs.qq.com/doc/DWXpKd0ZiWHJodVRV

负责实现ROS智能机器车的SLAM巡航、AI智能识别、警报提醒等功能。获得集创赛算能杯华南赛区二等奖。

搭建训练环境：使用VMware运行Ubuntu，安装ROS，通过ssh远程登录机器车的上位机开发板。在Windows上安装Docker并配置环境。

制作数据集：编写Python爬虫脚本爬取相关图片，结合使用roboflow网站制作数据集，使用labelImg标注数据集，在Colab用Yolov5算法进行训练。

量化：得到的结果在Docker中进行FP16量化，将得到的模型搭载到上位机主控板，实现AI智能识别。

使用激光雷达和深度摄像头获取数据实现A*导航算法以及各类硬件的调配与使用。

使用Python通过smtplib发送警报邮件。
