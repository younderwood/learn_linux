# 系统修复总结

一般操作系统无法进入多半由于软件冲突（即软件版本不兼容或软件包安装不完全等）



开机之后进入 Advanced Ubuntu recovery mode

之后进入 root terminal

开启网络链接：(只适用于wep模式)

- iwconfig 查看设备
- iwconfig dev ** scan | less
- iwconfig dev ** connect [网络名] 

网络连接上之后就可以运行：

- apt-get update

- apt-get upgrade

- apt autoremove

- apt-get dist-upgrade

- dkpt --configure -a

  ​

