Linux_STA_V2.5.0.3-32
====================================

修改os/linux/config.mk打开两个支持

代码:

# 打开Wpa_Supplicant

HAS_WPA_SUPPLICANT=y

# 打开网络管理器Native Wpa_Supplicant支持

HAS_NATIVE_WPA_SUPPLICANT_SUPPORT=y

#开始编译安装

1.打开终端一次输入以下代码

2.sudo su   注释：首次会让你输入密码

3.CD home/linuxidc/STA （注释：我是在终端里输入 cd 用鼠标把主文件下面刚复制进去的STA文件夹拖到终端里面的。这样就进入目录了吧。其他的我也不是很清楚，毕竟是业余的。）  也就是说进入home/linuxidc/STA

4.sudo make

5.sudo make install

6.sudo modprobe rt5370sta

到这基本上就能用了，保险一下步骤7。

7.添加到/etc/modules （没有进行次操作未发现异样。）

echo rt5370sta >> /etc/modules
