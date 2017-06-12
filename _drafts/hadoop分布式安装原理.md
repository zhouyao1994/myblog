---
layout: "post"
title: "hadoop分布式安装原理"
date: "2017-06-11 18:59"
---
# 搭建Hadoop步骤，以两个节点为例
1. 修改hosts给所有节点命名
2. 安装好java
2. ssh 免登录集群机器
3. 安装jdk，添加JAVA_HOME,复制Hadoop文件，修改权限
4. 在master节点的Hadoop文件目录Slaves上添加主机的ip
4. 在master节点的Hadoop文件目录core-site.xml修改tmp文件的目录
5. hdfs-site.xml修改备份的份数


## 拷贝到节点

## 解压缩到节点
```shell
sudo rm -rf /usr/local/hadoop/;sudo tar -zxf ~/hadoop.master.tar.gz -C /usr/local;sudo chown -R hadoop /usr/local/hadoop;

```
