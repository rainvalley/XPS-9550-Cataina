# XPS-9550-Cataina
[![YOVfw4.png](https://s1.ax1x.com/2020/05/22/YOVfw4.png)](https://imgchr.com/i/YOVfw4)
这是一份xps-9550在Catalina（macOS 10.15）下的引导，参考了repo：
* https://github.com/darkhandz/XPS15-9550-Catalina
* https://github.com/xzhih/one-key-hidpi
* https://github.com/zxystd/IntelBluetoothFirmware
* https://github.com/zxystd/itlwm

在此表示衷心的感谢！
# 配置
* 机型：xps-9550
* cpu，显卡：i7-6700hq hd530
* 网卡，蓝牙：Intel ac7265
* 声卡：realtek alc298
* 屏幕：夏普 3840*2160

# 完成度与问题
***我没有测试耳机插拔与hdmi相关的问题，如存在问题请自行打补丁，具体可参考[darkhandz/XPS15-9550-High-Sierra](https://github.com/darkhandz/XPS15-9550-High-Sierra)。***
## 完成内容
* 基本全部功能正常。
* Intel蓝牙正常驱动，Wi-Fi驱动暂时不建议直接加入kexts或者sle。
## 问题
* 如前文所述，Wi-Fi驱动不建议加入kexts，因此每次启动都需要kextload一遍。
* 插电时候的standby似乎有点问题，建议使用pmset关闭。
* 触摸屏不能使用，否则将会将系统从睡眠中唤醒。
* 重启之后有几率不能驱动触控板，使用tab+space可以选择重新启动。

# 相关问题
## 安装
我并不会提供安装具体流程，你可以参考[darkhandz/XPS15-9550-High-Sierra](https://github.com/darkhandz/XPS15-9550-High-Sierra)，我仅仅写了一篇补丁文章：https://blog.raincorn.top/2020/05/17/XPS_9550_mac/ 。
## Wi-Fi
请注意，Wi-Fi驱动只能在macOS 10.15上运行。我这里提供pcbeta一位吧友打包的脚本[[网卡] IntelWIFI 持续更新和自动开机连接WIFI驱动脚步包分享](http://bbs.pcbeta.com/viewthread-1856465-1-1.html)。如果需要最新版本的驱动，请参考[这里](https://github.com/zxystd/itlwm)自行编译。
## hidpi
运行Others文件夹下的hidpi.sh后重启即可。
## 洗白
建议先洗白后再登陆Apple ID，可以直接激活iMessage和FaceTime。
[![YOVwwQ.png](https://s1.ax1x.com/2020/05/22/YOVwwQ.png)](https://imgchr.com/i/YOVwwQ)

