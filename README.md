老版VNC  远程 Unable to connect to VNC Server using your chosen securitysetting

之所以出现这种问题是因为，远程连接Ubuntu桌面，在gnome桌面环境下，默认有一个VNC服务端 Vino，Vino需将安全认证关闭才能通过VNC Viewer连接。

通过以下命令可以关闭安全认证方式：
sudo gsettings set org.gnome.Vino require-encryption false

具体情况可以参考该博主
https://blog.csdn.net/chan1987818/article/details/126934283
