# ftp配置：
1. 首先打开终端,下载安装一下FTP服务器：sudo apt-get install vsftpd
2. 安装完成后查看一下版本：vsftps -v
3. 重启服务器：sudo reboot  
4. 打开配置文件在最后的末尾加上这几条语句：
  ```
  anonymous_enable=YES
  anon_root=/home/xinwenpeng/ftp
  no_anon_password=YES
  write_enable=YES 
  anon_upload_enable=YES 
  anon_mkdir_write_enable=YES
  ```
  配置文件地址: 
  > https://github.com/Franklin-F/raspberry-config/blob/master/vsftpd.conf
5. 启动 sudo /etc/init.d/vsftpd restart
6. 教程：https://www.ituring.com.cn/article/273666