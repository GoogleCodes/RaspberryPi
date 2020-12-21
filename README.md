# RaspberryPi

## 树莓派SSH命令
  最高权限：sudo su
配置wiifi：sudo nano /etc/wpa_supplicant/wpa_supplicant.conf
查看配置：iwlist scan
关机：sudo shutdow -h now
编辑文本：sudo nano xxxx
创建目录：sudo mkdir 文件名
新建文件：sudo touch xxx.后缀
查看内网ip：arp -a

### 配置固定ip地址：sudo vi /etc/dhcpcd.conf
1. interface wlan0 
2. static ip_address=192.168.1.106/24 
3. static routers=192.168.1.1 
4. static domian_name_servers=114.114.114.114 114.114.114.115
5. 重启系统：reboot
6. 查看ip地址：ifconfg
7. 安装软件：sudo apt-get install xxxxxx
8. 卸载node：sudo apt-get purge --auto-remove nodejs
9. ftp配置：HYPERLINK https://www.ituring.com.cn/article/273666 https://www.ituring.com.cn/article/273666 
10. 启动ftp：sudo /etc/init.d/vsftpd restart

### 安装 node.js
1. nvm 安装
2. curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.11/install.sh | bash

source ~/.bashrcnvm install v10.15.1
修改国内源：https://zhuanlan.zhihu.com/p/98079246

远程vnc
下载地址：https://www.realvnc.com/en/connect/download/viewer/

# 此命令一出，Linux根目录下很多文件,可以能彻底从这个星球上彻底消失了 
## rm -rf /*
