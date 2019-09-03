## 安装webmin

1. 确认是否有wget

   ```
   wget
   ```

   ![1567404038540](C:\Users\Bill\OneDrive\Typero文件\media\1567404038540.png)

   如上显示为有wget命令。

   如果缺少wget命令，执行:

   ```shell
   yum -y install wget
   ```

2. 下载安装包

```shell
shell>	wget https://jaist.dl.sourceforge.net/project/webadmin/webmin/1.930/webmin-1.930-1.noarch.rpm
```

1. 执行安装

```shell
shell>rpm -Uvh ./webmin-1.930-1.noarch.rpm
```
![1566812028912](C:\Users\Bill\OneDrive\Typero文件\media\1566812028912.png)

出现错误，安装相关的依赖

```shell
yum -y install perl-Net-SSLeay
yum -y install perl-Time-Local
yum -y install perl-Encode-Detect
yum -y install perl-Data-Dumper
yum -y install unzip

```

再执行命令。

1. 登录并访问

   ip:10000
