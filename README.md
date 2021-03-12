This project is developed using Tuya SDK, which enables you to quickly develop branded apps connecting and controlling smart scenarios of many devices. For mor information, please check Tuya Developer Website.
# 一、方案标题
智能宠物投食器
# 二、方案应用场景
主要用于宠物独自在家无人照顾，解决主人担忧
功能：1.通过wifi模块连入涂鸦网络平台进行管理
      2.可通过手机APP可手动在屏幕上选择，定时、定量对宠物进行投喂等操作
      3.可通过手机APP或者LCD屏查看喂食、余粮等信息记录
      4.余粮不足提示告警
      5.对投喂剩余粮进行自动清理
      6.将涂鸦wifi摄像头接入wifi,通过APP可以视频监控查看
# 三、技术方案
主控选择STM32F103外加一块从机Arduino，外设包括需要投喂的宠物粮以及控制的电机，称余粮的压力传感器，显示菜单的LCD屏幕，需要告警的LED灯或者蜂鸣器，涂鸦wifi摄像头，在食槽底部安装压力传感器检测食物信号。通过涂鸦的WIFI模组联网，通过串口将单片机数据和云端数据交互，来完成一系列的命令下发上传的。从机主要来做实际电机控制，主机收到云端下发命令后通过串口告知从机进行动作执行。
# 四、开发计划
3月30前完成.
1. 3月8前准备物料 看官方SDK
2. 3月9-3月12日跑SDK例程 熟悉SDK
3. 3月13-3月19嵌入式开发、云开发
4. 3月20-3月26 3D外壳设计 整机调试
5. 3月29日前整体调试。
