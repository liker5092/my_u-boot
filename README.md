# my_u-boot
openwrt u-boot list


## 1
高通IPQ系列定制U-Boot，源自开源的QSDK 12.5。支持以下功能：

集成U-Boot的webfailsafe模式

集成DHCP服务

集成Web页面修改环境变量

支持U-Boot更新、固件更新、CDT更新、MIBIB更新、GPT更新、ART更新、initramfs启动进行调试和恢复
支持在环境变量中自定义reset_key=<GPIO_NUM>，（覆盖模式）以方便在没有添加支持的设备上启用按压reset按键进入uboot的webfailsafe模式进行相应的升级操作
设置方法：①ttl下输入
'setenv reset_key x && saveenv'
设置方法：②或者环境变量页面变量名框中输入'reset_key',变量值框中输入'x'，然后点'修改变量'重启后永久生效
注：'x'为你已知的gpio值。
支持在环境变量中自定义config_name=config@xxx，（覆盖模式）以方便夸机型，夸型号，夸固件进行测试
设置方法：①ttl下输入‘setenv config_name config@x && saveenv’
设置方法：②或者环境变量页面变量名框中输入'config_name',在变量值框中输入'config@xxx'，然后点‘修改变量’重启后永久生效
取消覆盖的变量名以及值reset_key/config_name，在ttl下输入'setenv reset_key''saveenv' / 'setenv config_name''saveenv'重启即调用dtb中的默认条目

[https://github.com/1980490718/u-boot-2016]

## 2
此项目已适配以下 IPQ60xx eMMC 机型：老板说基本 1 的大佬
支持

京东云太乙（RE-CS-07）

京东云亚瑟（RE-SS-01）

京东云雅典娜（RE-CS-02）

连我 NN6000（V1 & V2）

红米 AX5 JDCloud（RA50）


[https://github.com/chenxin527/uboot-ipq60xx-emmc-build]
