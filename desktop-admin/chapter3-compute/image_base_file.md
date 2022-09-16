## 3.2 镜像文件

镜像文件类似于装系统的IOS文件,运营后台统一管理。镜像制作人员将镜像文件制作完毕之后可以上传至FTP文件服务器，运营后台会提供文件服务器的IP、端口、用户、密码，镜像文件制作人员使用客户端登录上传即可，两种方法：  
**1. windows端**  
客户端使用FileZilla，下载地址：[https://www.filezilla.cn/download/client](https://www.filezilla.cn/download/client) ,可以下载64位绿色安装版。  
上传文件的IP和端口可以在自动化部署的时候指定，默认的用户和密码是admin，admin。  
**2. linux端**  
使用ftp命令  
如下图：

在put文件之前记得执行binary命令，这样上传的文件就会保持一致，MD5值不会改变。

![](/assets/linux-ftp.png)

镜像制作人员将镜像文件上传之后，在运营后台点击“同步”，可以获取镜像文件列表。

![](/assets/image-base.png)

选取需要发布的镜像文件，点击发布，选择集群，就可以将该镜像文件发布到OS集群。发布镜像的过程需要花费一段时间，带宽越好，速度越快，一般需要7分钟左右。

![](/assets/imag-fabu.png)![](/assets/iamge-fabu2.png)

**注：** 
这里有一个镜像文件必须发布到OS集群，不然无法创建数据盘，镜像文件的名字为：Windows-Data-Disk-NTFS-1G.qcow2，大小为8MB。

