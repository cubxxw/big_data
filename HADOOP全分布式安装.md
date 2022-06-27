## Linux环境准备

修改主机名：hostname

| 192.168.16.142 | 192.168.16.51 | 192.168.16.76 |
| -------------- | ------------- | ------------- |
| master         | slave1        | slave2        |

配置action-1的映射文件：vi /etc/hosts

将action-1的hosts文件上传到其他两个节点：

scp  /etc/hosts action-2:/etc/

ssh配置：

密钥生成命令：ssh-keygen

将action-1的公钥拷贝到三个节点上

拷贝密钥：ssh-copy-id action-1、ssh-copy-id action-2、ssh-copy-id action-3

测试免密是否成功：

ssh action-2

临时关闭防火墙：systemctl stop firewalld

永久关闭防火墙：systemctl disable firewalld

### jdk安装

略

## HADOOP全分布式安装

**修改core-site.xml配置文件**

```xml
<configuration>
    <property>
        <name>hadoop.tmp.dir</name>
        <value>/usr/local/src/hadoop/tmp</value>
        <description>Abase for other temporary directories.</description>
    </property>
    <property>
        <name>fs.defaultFS</name>
        <value>hdfs://master:9000</value>
    </property>
</configuration>
```

**修改hdfs-site.xml配置文件**

```xml
<configuration>
  <property>
     <name>dfs.replication</name>
     <value>2</value>
  </property>
</configuration>
```

**修改mapred-site.xml配置文件**

```xml
<property>
    <name>mapreduce.framework.name</name>
    <value>yarn</value>
</property>
<property>
    <name>mapreduce.jobhistory.address</name>
    <value>hadoop01:10020</value>
</property>
<property>
    <name>mapreduce.jobhistory.webapp.address</name>
    <value>hadoop02:19888</value>
</property>
```

**修改yarn-site.xml配置文件**

```xml
<property>
    <name>yarn.nodemanager.aux-services</name>
    <value>mapreduce_shuffle</value>
</property>
<property>
    <name>yarn.resourcemanager.hostname</name>
    <value>hadoop01</value>
</property>
<property>
    <name>yarn.log-aggregation-enable</name>
    <value>true</value>
</property>
<property>
    <name>yarn.log-aggregation.retain-seconds</name>
    <value>106800</value>
</property>
```

**修改hadoop-env.sh**

修改jdk的绝对路径

**配置slaves文件**

(1)配置master文件如下：

master

slave1

slave2

#### 添加hadoop 环境变量

略

### 同传

scp -r [本机的文件或文件夹] action-2：[路径]

### 初始化命令

hadoop namenode -format

### 启动命令：

start-dfs.sh和start-yarn.sh

启动历史进程：mr-jobhistory-daemon.sh start historyserver

### 验证是否启动以下进程

**action-1:** 

- NameNode
- DataNode
- ResourceManager
- NodeManager
- SecondaryNameNode
- JobHistoryServer



**action-2:** 

- DataNode
- NodeManager



**action-3:**

- DataNode

- NodeManager

  ### 查看各种管理界面

  namenode管理界面：http://ip:50070

  datanode管理界面：http://ip:50075

  yarn管理界面：http://ip:8088

  任务历史查看界面：http://ip:19888

### 其他

Namenode 管理者文件系统

Datanode是文件系统

Secondary NameNode是一个用来监控HDFS状态的辅助后台程序

JobTracker后台程序用来连接应用程序与Hadoop





