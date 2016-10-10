# 常用命令

## top

按数字键“1”就可以看到每个核心的使用情况

## 压缩、解压

.tar.gz

```
tar -cvzf filename.tar.gz /home/yanjie
tar -zxvf filename.tar.gz
```

## yum

```
yum list available tomcat* //列出可以安装的tomcat包
```

## 自启动

```
chkconfig vsftpd on
```

# CentOS 7

## 最小安装，激活网卡

```
# ls /etc/sysconfig/network-scripts
# vi /etc/sysconfig/network-scripts/ifcfg-epn0s3
将其中的ONBOOT改为yes
# service network start
```
