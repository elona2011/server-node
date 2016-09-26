# 常用命令

## top

按数字键“1”就可以看到每个核心的使用情况

## tar

.tar.gz

```
tar -zxv -f filename.tar.gz
```

# CentOS 7

## 最小安装，激活网卡

```
# ls /etc/sysconfig/network-scripts
# vi /etc/sysconfig/network-scripts/ifcfg-epn0s3
将其中的ONBOOT改为yes
# service network start
```
