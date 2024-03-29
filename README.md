﻿# 大数据笔记和配置

### [hadoop详细文档讲解下载](hadooop详解.docx)



## TOC

#### 1. [hadoop教程](markdown/1.md)

#### 2. [Hadoop 运行环境](markdown/2.md)

#### 3. [Hadoop 概念](markdown/3.md)

#### 4. [HDFS 配置与使用](markdown/4.md)

#### 5. [HDFS 集群](markdown/5.md)

#### 6. [MapReduce 使用](markdown/6.md)

#### 7. [MapReduce 编程](markdown/7.md)

#### 8. [基本环境](markdown/8.md)

#### 9. [hadoop运行模式](markdown/9.md)

#### 10. [配置ssh](markdown/10.md)

#### 11. [配置ip](markdown/11.md)

#### 12. [三个虚拟机的配置](markdown/12.md)

#### 13. [集群配置](markdown/13.md)

#### 14. [配置ip](markdown/14.md)

#### 15. [配置历史服务器](markdown/15.md)

#### 


## 补充：关于 Kubernetes 部署 hadoop 方法

**部署 Kubernetes 的集群：**
```bash
sudo /home/sealer/sealer2/_output/bin/sealer/linux_amd64/sealer run docker.io/sealerio/kubernetes:v1.22.15 --masters 10.0.0.245 --nodes 10.0.0.246,10.0.0.247  --user sealer --passwd ********
```


**Hadoop镜像，到docker hub上拉取：**
```bash
docker pull kubeguide/hadoop:latest
```

**编辑 hadoop.yaml 文件：**
```yaml
apiVersion: v1
kind: ConfigMap
metadata:
  name: kube-hadoop-conf
  namespace: default
data:
  HDFS_MASTER_SERVICE: hadoop-hdfs-master
  HDOOP_YARN_MASTER: hadoop-yarn-master
---
apiVersion: v1
kind: Service
metadata:
  name: hadoop-hdfs-master
spec:
  type: NodePort
  selector:
    app: hdfs-master
  ports:
    - name: rpc
      port: 9000
      targetPort: 9000
    - name: http
      port: 50070
      targetPort: 50070
      nodePort: 32007
---
apiVersion: v1
kind: Pod
metadata:
  name: hdfs-master
  labels:
    app: hdfs-master
spec:
  containers:
    - name: hdfs-master
      image: 192.168.242.132/library/kubernetes-hadoop:latest
      imagePullPolicy: IfNotPresent
      ports:
        - containerPort: 9000
        - containerPort: 50070    
      env:
        - name: HADOOP_NODE_TYPE
          value: namenode
        - name: HDFS_MASTER_SERVICE
          valueFrom:
            configMapKeyRef:
              name: kube-hadoop-conf
              key: HDFS_MASTER_SERVICE
        - name: HDOOP_YARN_MASTER
          valueFrom:
            configMapKeyRef:
              name: kube-hadoop-conf
              key: HDOOP_YARN_MASTER
  restartPolicy: Always
---
apiVersion: v1
kind: Pod
metadata:
    name: hadoop-datanode-1
    labels:
      app: hadoop-datanode-1
spec:
  containers:
    - name: hadoop-datanode-1
      image: 192.168.242.132/library/kubernetes-hadoop:latest
      imagePullPolicy: IfNotPresent
      ports:
        - containerPort: 9000
        - containerPort: 50070    
      env:
        - name: HADOOP_NODE_TYPE
          value: datanode
        - name: HDFS_MASTER_SERVICE
          valueFrom:
            configMapKeyRef:
              name: kube-hadoop-conf
              key: HDFS_MASTER_SERVICE
        - name: HDOOP_YARN_MASTER
          valueFrom:
            configMapKeyRef:
              name: kube-hadoop-conf
              key: HDOOP_YARN_MASTER        
  restartPolicy: Always
---
apiVersion: v1
kind: Pod
metadata:
    name: hadoop-datanode-2
    labels:
      app: hadoop-datanode-2
spec:
  containers:
    - name: hadoop-datanode-2
      image: 192.168.242.132/library/kubernetes-hadoop:latest
      imagePullPolicy: IfNotPresent
      ports:
        - containerPort: 9000
        - containerPort: 50070    
      env:
        - name: HADOOP_NODE_TYPE
          value: datanode
        - name: HDFS_MASTER_SERVICE
          valueFrom:
            configMapKeyRef:
              name: kube-hadoop-conf
              key: HDFS_MASTER_SERVICE
        - name: HDOOP_YARN_MASTER
          valueFrom:
            configMapKeyRef:
              name: kube-hadoop-conf
              key: HDOOP_YARN_MASTER        
  restartPolicy: Always
---
apiVersion: v1
kind: Pod
metadata:
    name: hadoop-datanode-3
    labels:
      app: hadoop-datanode-3
spec:
  containers:
    - name: hadoop-datanode-3
      image: 192.168.242.132/library/kubernetes-hadoop:latest
      imagePullPolicy: IfNotPresent
      ports:
        - containerPort: 9000
        - containerPort: 50070    
      env:
        - name: HADOOP_NODE_TYPE
          value: datanode
        - name: HDFS_MASTER_SERVICE
          valueFrom:
            configMapKeyRef:
              name: kube-hadoop-conf
              key: HDFS_MASTER_SERVICE
        - name: HDOOP_YARN_MASTER
          valueFrom:
            configMapKeyRef:
              name: kube-hadoop-conf
              key: HDOOP_YARN_MASTER        
  restartPolicy: Always
---
apiVersion: v1
kind: Service
metadata:
  name: hadoop-yarn-master
spec:
  type: NodePort
  selector:
    app: yarn-master
  ports:
     - name: "8030"       
       port: 8030
     - name: "8031"     
       port: 8031
     - name: "8032"
       port: 8032     
     - name: http
       port: 8088
       targetPort: 8088
       nodePort: 32088
---
apiVersion: v1
kind: Pod
metadata:
  name: yarn-master
  labels:
    app: yarn-master
spec:
  containers:
    - name: yarn-master
      image: 192.168.242.132/library/kubernetes-hadoop:latest
      imagePullPolicy: IfNotPresent
      ports:
        - containerPort: 9000
        - containerPort: 50070    
      env:
        - name: HADOOP_NODE_TYPE
          value: resourceman
        - name: HDFS_MASTER_SERVICE
          valueFrom:
            configMapKeyRef:
              name: kube-hadoop-conf
              key: HDFS_MASTER_SERVICE
        - name: HDOOP_YARN_MASTER
          valueFrom:
            configMapKeyRef:
              name: kube-hadoop-conf
              key: HDOOP_YARN_MASTER          
  restartPolicy: Always
---
apiVersion: v1
kind: Service
metadata:
  name: yarn-node-1
spec:
  clusterIP: None
  selector:
    app: yarn-node-1
  ports:
     - port: 8040
---
apiVersion: v1
kind: Service
metadata:
  name: yarn-node-2
spec:
  clusterIP: None
  selector:
    app: yarn-node-2
  ports:
     - port: 8040
---
apiVersion: v1
kind: Service
metadata:
  name: yarn-node-3
spec:
  clusterIP: None
  selector:
    app: yarn-node-3
  ports:
     - port: 8040
---
apiVersion: v1
kind: Pod
metadata:
  name: yarn-node-1
  labels:
    app: yarn-node-1
spec:
  containers:
    - name: yarn-node-1
      image: 192.168.242.132/library/kubernetes-hadoop:latest
      imagePullPolicy: IfNotPresent
      ports:
        - containerPort: 8040
        - containerPort: 8041   
        - containerPort: 8042        
      env:
        - name: HADOOP_NODE_TYPE
          value: yarnnode
        - name: HDFS_MASTER_SERVICE
          valueFrom:
            configMapKeyRef:
              name: kube-hadoop-conf
              key: HDFS_MASTER_SERVICE
        - name: HDOOP_YARN_MASTER
          valueFrom:
            configMapKeyRef:
              name: kube-hadoop-conf
              key: HDOOP_YARN_MASTER          
  restartPolicy: Always
---
apiVersion: v1
kind: Pod
metadata:
  name: yarn-node-2
  labels:
    app: yarn-node-2
spec:
  containers:
    - name: yarn-node-2
      image: 192.168.242.132/library/kubernetes-hadoop:latest
      imagePullPolicy: IfNotPresent
      ports:
        - containerPort: 8040
        - containerPort: 8041   
        - containerPort: 8042        
      env:
        - name: HADOOP_NODE_TYPE
          value: yarnnode
        - name: HDFS_MASTER_SERVICE
          valueFrom:
            configMapKeyRef:
              name: kube-hadoop-conf
              key: HDFS_MASTER_SERVICE
        - name: HDOOP_YARN_MASTER
          valueFrom:
            configMapKeyRef:
              name: kube-hadoop-conf
              key: HDOOP_YARN_MASTER          
  restartPolicy: Always
---
apiVersion: v1
kind: Pod
metadata:
  name: yarn-node-3
  labels:
    app: yarn-node-3
spec:
  containers:
    - name: yarn-node-3
      image: 192.168.242.132/library/kubernetes-hadoop:latest
      imagePullPolicy: IfNotPresent
      ports:
        - containerPort: 8040
        - containerPort: 8041   
        - containerPort: 8042        
      env:
        - name: HADOOP_NODE_TYPE
          value: yarnnode
        - name: HDFS_MASTER_SERVICE
          valueFrom:
            configMapKeyRef:
              name: kube-hadoop-conf
              key: HDFS_MASTER_SERVICE
        - name: HDOOP_YARN_MASTER
          valueFrom:
            configMapKeyRef:
              name: kube-hadoop-conf
              key: HDOOP_YARN_MASTER          
  restartPolicy: Always
```
> 这个yaml文件包含一个ConfigMap，5个Service，8个pod，这里需要注意的是ConfigMap中HDFS_MASTER_SERVICE和HDOOP_YARN_MASTER不要使用IP，使用HDFS service的名称，否则datanode将会连接不上namenode，出现错误【ipc.Client: Retrying connect to server: xxx:9000.】

**创建命令：**
```bash
kubectl create -f hadoop.yaml
```

## else

> 2022年6月27日 18:49:58

```bash

    目录: C:\Users\smile\Desktop\git\big-date


Mode                 LastWriteTime         Length Name                                                                 
----                 -------------         ------ ----
d-----         2022/6/27     18:48                markdowm                                                             
-a----         2022/6/27     18:45        4957395 hadooop详解.docx                                                       
-a----         2022/6/27     18:45        3870121 hadoop.zip                                                           
-a----          2022/4/8     15:58           3275 HADOOP全分布式安装.md                                                      
-a----         2022/6/27     18:49             56 README.md                                                            
-a----          2022/4/4     21:42          70002 solution.md                                                          
-a----         2022/6/27     18:45              0 TOC.md                                                               
-a----         2022/6/27     18:45           2279 配置文件.md                                                              
-a----         2022/6/27     18:45          43376 集群.md                                                                

```
