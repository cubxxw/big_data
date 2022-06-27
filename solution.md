

## 我的操作 – Hadoop01

```shell
cd /opt
[root@hadoop01 ~]# cd /opt
[root@hadoop01 opt]# vi /etc/profile.d/my_path.sh 
[root@hadoop01 opt]# source /e
etc/    export/ 
[root@hadoop01 opt]# source /etc/profile.d/my_path.sh 
[root@hadoop01 opt]# scp /e
/etc/     /export/  
[root@hadoop01 opt]# scp /etc/profile.d/my_path.sh hadoop02:/e
/etc/     /export/  
[root@hadoop01 opt]# scp /etc/profile.d/my_path.sh hadoop02:/e
/etc/     /export/  
[root@hadoop01 opt]# scp /etc/profile.d/my_path.sh hadoop02:/etc/profile.d/my_path.sh 
my_path.sh                                                     100%  543   351.7KB/s   00:00    
[root@hadoop01 opt]# scp /etc/profile.d/my_path.sh hadoop03:/etc/profile.d/my_path.sh 
my_path.sh                                                     100%  543   537.6KB/s   00:00    
[root@hadoop01 opt]# hadoop 
adoptopenjdk-11-hotspot-11.0.10+9-3.x86_64.rpm  hadoop-3.3.2/
[root@hadoop01 opt]# hadoop namenode -format
WARNING: Use of this script to execute namenode is deprecated.
WARNING: Attempting to execute replacement "hdfs namenode" instead.

2022-04-03 08:38:52,435 INFO namenode.NameNode: STARTUP_MSG: 
/************************************************************
STARTUP_MSG: Starting NameNode
STARTUP_MSG:   host = hadoop01/192.168.121.134
STARTUP_MSG:   args = [-format]
STARTUP_MSG:   version = 3.3.2
STARTUP_MSG:   classpath = /opt/hadoop-3.3.2//etc/hadoop:/opt/hadoop-3.3.2//share/hadoop/common/lib/accessors-smart-2.4.7.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/animal-sniffer-annotations-1.17.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/asm-5.0.4.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/audience-annotations-0.5.0.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/avro-1.7.7.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/checker-qual-2.5.2.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/commons-beanutils-1.9.4.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/commons-cli-1.2.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/commons-codec-1.11.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/commons-collections-3.2.2.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/commons-compress-1.21.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/commons-configuration2-2.1.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/commons-daemon-1.0.13.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/commons-io-2.8.0.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/commons-lang3-3.12.0.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/commons-logging-1.1.3.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/commons-math3-3.1.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/commons-net-3.6.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/commons-text-1.4.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/curator-client-4.2.0.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/curator-framework-4.2.0.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/curator-recipes-4.2.0.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/dnsjava-2.1.7.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/failureaccess-1.0.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/gson-2.8.9.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/guava-27.0-jre.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/hadoop-annotations-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/hadoop-auth-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/hadoop-shaded-guava-1.1.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/hadoop-shaded-protobuf_3_7-1.1.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/httpclient-4.5.13.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/httpcore-4.4.13.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/j2objc-annotations-1.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jackson-annotations-2.13.0.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jackson-core-2.13.0.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jackson-core-asl-1.9.13.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jackson-databind-2.13.0.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jackson-jaxrs-1.9.13.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jackson-mapper-asl-1.9.13.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jackson-xc-1.9.13.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jakarta.activation-api-1.2.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/javax.servlet-api-3.1.0.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jaxb-api-2.2.11.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jaxb-impl-2.2.3-1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jcip-annotations-1.0-1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jersey-core-1.19.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jersey-json-1.19.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jersey-server-1.19.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jersey-servlet-1.19.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jettison-1.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jetty-http-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jetty-io-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jetty-security-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jetty-server-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jetty-servlet-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jetty-util-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jetty-util-ajax-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jetty-webapp-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jetty-xml-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jsch-0.1.55.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/json-smart-2.4.7.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jsp-api-2.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jsr305-3.0.2.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jsr311-api-1.1.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jul-to-slf4j-1.7.30.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerb-admin-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerb-client-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerb-common-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerb-core-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerb-crypto-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerb-identity-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerb-server-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerb-simplekdc-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerb-util-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerby-asn1-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerby-config-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerby-pkix-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerby-util-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerby-xdr-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/listenablefuture-9999.0-empty-to-avoid-conflict-with-guava.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/log4j-1.2.17.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/metrics-core-3.2.4.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/netty-3.10.6.Final.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/nimbus-jose-jwt-9.8.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/paranamer-2.3.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/protobuf-java-2.5.0.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/re2j-1.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/slf4j-api-1.7.30.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/slf4j-log4j12-1.7.30.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/snappy-java-1.1.8.2.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/stax2-api-4.2.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/token-provider-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/woodstox-core-5.3.0.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/zookeeper-3.5.6.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/zookeeper-jute-3.5.6.jar:/opt/hadoop-3.3.2//share/hadoop/common/hadoop-common-3.3.2-tests.jar:/opt/hadoop-3.3.2//share/hadoop/common/hadoop-common-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/common/hadoop-kms-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/common/hadoop-nfs-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/common/hadoop-registry-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/accessors-smart-2.4.7.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/animal-sniffer-annotations-1.17.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/asm-5.0.4.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/audience-annotations-0.5.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/avro-1.7.7.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/checker-qual-2.5.2.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/commons-beanutils-1.9.4.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/commons-cli-1.2.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/commons-codec-1.11.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/commons-collections-3.2.2.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/commons-compress-1.21.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/commons-configuration2-2.1.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/commons-daemon-1.0.13.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/commons-io-2.8.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/commons-lang3-3.12.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/commons-logging-1.1.3.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/commons-math3-3.1.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/commons-net-3.6.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/commons-text-1.4.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/curator-client-4.2.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/curator-framework-4.2.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/curator-recipes-4.2.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/dnsjava-2.1.7.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/failureaccess-1.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/gson-2.8.9.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/guava-27.0-jre.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/hadoop-annotations-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/hadoop-auth-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/hadoop-shaded-guava-1.1.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/hadoop-shaded-protobuf_3_7-1.1.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/httpclient-4.5.13.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/httpcore-4.4.13.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/j2objc-annotations-1.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jackson-annotations-2.13.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jackson-core-2.13.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jackson-core-asl-1.9.13.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jackson-databind-2.13.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jackson-jaxrs-1.9.13.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jackson-mapper-asl-1.9.13.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jackson-xc-1.9.13.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jakarta.activation-api-1.2.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/javax.servlet-api-3.1.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jaxb-api-2.2.11.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jaxb-impl-2.2.3-1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jcip-annotations-1.0-1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jersey-core-1.19.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jersey-json-1.19.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jersey-server-1.19.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jersey-servlet-1.19.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jettison-1.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jetty-http-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jetty-io-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jetty-security-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jetty-server-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jetty-servlet-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jetty-util-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jetty-util-ajax-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jetty-webapp-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jetty-xml-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jsch-0.1.55.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/json-simple-1.1.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/json-smart-2.4.7.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jsr305-3.0.2.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jsr311-api-1.1.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerb-admin-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerb-client-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerb-common-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerb-core-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerb-crypto-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerb-identity-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerb-server-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerb-simplekdc-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerb-util-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerby-asn1-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerby-config-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerby-pkix-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerby-util-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerby-xdr-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/leveldbjni-all-1.8.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/listenablefuture-9999.0-empty-to-avoid-conflict-with-guava.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/log4j-1.2.17.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/netty-3.10.6.Final.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/netty-all-4.1.68.Final.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/nimbus-jose-jwt-9.8.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/okhttp-2.7.5.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/okio-1.6.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/paranamer-2.3.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/protobuf-java-2.5.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/re2j-1.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/snappy-java-1.1.8.2.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/stax2-api-4.2.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/token-provider-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/woodstox-core-5.3.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/zookeeper-3.5.6.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/zookeeper-jute-3.5.6.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/hadoop-hdfs-3.3.2-tests.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/hadoop-hdfs-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/hadoop-hdfs-client-3.3.2-tests.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/hadoop-hdfs-client-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/hadoop-hdfs-httpfs-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/hadoop-hdfs-native-client-3.3.2-tests.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/hadoop-hdfs-native-client-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/hadoop-hdfs-nfs-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/hadoop-hdfs-rbf-3.3.2-tests.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/hadoop-hdfs-rbf-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/mapreduce/hadoop-mapreduce-client-app-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/mapreduce/hadoop-mapreduce-client-common-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/mapreduce/hadoop-mapreduce-client-core-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/mapreduce/hadoop-mapreduce-client-hs-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/mapreduce/hadoop-mapreduce-client-hs-plugins-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/mapreduce/hadoop-mapreduce-client-jobclient-3.3.2-tests.jar:/opt/hadoop-3.3.2//share/hadoop/mapreduce/hadoop-mapreduce-client-jobclient-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/mapreduce/hadoop-mapreduce-client-nativetask-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/mapreduce/hadoop-mapreduce-client-shuffle-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/mapreduce/hadoop-mapreduce-client-uploader-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/mapreduce/hadoop-mapreduce-examples-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/HikariCP-java7-2.4.12.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/aopalliance-1.0.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/asm-analysis-9.1.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/asm-commons-9.1.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/asm-tree-9.1.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/bcpkix-jdk15on-1.60.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/bcprov-jdk15on-1.60.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/ehcache-3.3.1.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/fst-2.50.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/geronimo-jcache_1.0_spec-1.0-alpha-1.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/guice-4.0.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/guice-servlet-4.0.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/jackson-jaxrs-base-2.13.0.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/jackson-jaxrs-json-provider-2.13.0.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/jackson-module-jaxb-annotations-2.13.0.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/jakarta.xml.bind-api-2.3.3.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/java-util-1.9.0.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/javax-websocket-client-impl-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/javax-websocket-server-impl-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/javax.inject-1.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/javax.websocket-api-1.0.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/javax.websocket-client-api-1.0.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/javax.ws.rs-api-2.1.1.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/jersey-client-1.19.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/jersey-guice-1.19.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/jetty-annotations-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/jetty-client-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/jetty-jndi-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/jetty-plus-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/jline-3.9.0.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/jna-5.2.0.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/json-io-2.5.1.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/metrics-core-3.2.4.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/mssql-jdbc-6.2.1.jre7.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/objenesis-2.6.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/snakeyaml-1.26.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/swagger-annotations-1.5.4.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/websocket-api-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/websocket-client-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/websocket-common-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/websocket-server-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/websocket-servlet-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-api-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-applications-distributedshell-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-applications-mawo-core-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-applications-unmanaged-am-launcher-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-client-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-common-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-registry-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-server-applicationhistoryservice-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-server-common-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-server-nodemanager-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-server-resourcemanager-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-server-router-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-server-sharedcachemanager-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-server-tests-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-server-timeline-pluginstorage-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-server-web-proxy-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-services-api-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-services-core-3.3.2.jar
STARTUP_MSG:   build = git@github.com:apache/hadoop.git -r 0bcb014209e219273cb6fd4152df7df713cbac61; compiled by 'chao' on 2022-02-21T18:39Z
STARTUP_MSG:   java = 11.0.1
************************************************************/
2022-04-03 08:38:52,463 INFO namenode.NameNode: registered UNIX signal handlers for [TERM, HUP, INT]
2022-04-03 08:38:52,641 INFO namenode.NameNode: createNameNode [-format]
2022-04-03 08:38:53,416 INFO namenode.NameNode: Formatting using clusterid: CID-79c95162-7312-4b0c-ad64-b73a7be27da2
2022-04-03 08:38:53,476 INFO namenode.FSEditLog: Edit logging is async:true
2022-04-03 08:38:53,537 INFO namenode.FSNamesystem: KeyProvider: null
2022-04-03 08:38:53,538 INFO namenode.FSNamesystem: fsLock is fair: true
2022-04-03 08:38:53,538 INFO namenode.FSNamesystem: Detailed lock hold time metrics enabled: false
2022-04-03 08:38:53,602 INFO namenode.FSNamesystem: fsOwner                = root (auth:SIMPLE)
2022-04-03 08:38:53,602 INFO namenode.FSNamesystem: supergroup             = supergroup
2022-04-03 08:38:53,602 INFO namenode.FSNamesystem: isPermissionEnabled    = true
2022-04-03 08:38:53,602 INFO namenode.FSNamesystem: isStoragePolicyEnabled = true
2022-04-03 08:38:53,603 INFO namenode.FSNamesystem: HA Enabled: false
2022-04-03 08:38:53,724 INFO common.Util: dfs.datanode.fileio.profiling.sampling.percentage set to 0. Disabling file IO profiling
2022-04-03 08:38:53,748 INFO blockmanagement.DatanodeManager: dfs.block.invalidate.limit: configured=1000, counted=60, effected=1000
2022-04-03 08:38:53,748 INFO blockmanagement.DatanodeManager: dfs.namenode.datanode.registration.ip-hostname-check=true
2022-04-03 08:38:53,751 INFO blockmanagement.BlockManager: dfs.namenode.startup.delay.block.deletion.sec is set to 000:00:00:00.000
2022-04-03 08:38:53,752 INFO blockmanagement.BlockManager: The block deletion will start around 2022 Apr 03 08:38:53
2022-04-03 08:38:53,754 INFO util.GSet: Computing capacity for map BlocksMap
2022-04-03 08:38:53,754 INFO util.GSet: VM type       = 64-bit
2022-04-03 08:38:53,757 INFO util.GSet: 2.0% max memory 452 MB = 9.0 MB
2022-04-03 08:38:53,757 INFO util.GSet: capacity      = 2^20 = 1048576 entries
2022-04-03 08:38:53,780 INFO blockmanagement.BlockManager: Storage policy satisfier is disabled
2022-04-03 08:38:53,781 INFO blockmanagement.BlockManager: dfs.block.access.token.enable = false
2022-04-03 08:38:53,790 INFO blockmanagement.BlockManagerSafeMode: dfs.namenode.safemode.threshold-pct = 0.999
2022-04-03 08:38:53,790 INFO blockmanagement.BlockManagerSafeMode: dfs.namenode.safemode.min.datanodes = 0
2022-04-03 08:38:53,790 INFO blockmanagement.BlockManagerSafeMode: dfs.namenode.safemode.extension = 30000
2022-04-03 08:38:53,791 INFO blockmanagement.BlockManager: defaultReplication         = 3
2022-04-03 08:38:53,791 INFO blockmanagement.BlockManager: maxReplication             = 512
2022-04-03 08:38:53,791 INFO blockmanagement.BlockManager: minReplication             = 1
2022-04-03 08:38:53,791 INFO blockmanagement.BlockManager: maxReplicationStreams      = 2
2022-04-03 08:38:53,791 INFO blockmanagement.BlockManager: redundancyRecheckInterval  = 3000ms
2022-04-03 08:38:53,791 INFO blockmanagement.BlockManager: encryptDataTransfer        = false
2022-04-03 08:38:53,791 INFO blockmanagement.BlockManager: maxNumBlocksToLog          = 1000
2022-04-03 08:38:53,824 INFO namenode.FSDirectory: GLOBAL serial map: bits=29 maxEntries=536870911
2022-04-03 08:38:53,824 INFO namenode.FSDirectory: USER serial map: bits=24 maxEntries=16777215
2022-04-03 08:38:53,824 INFO namenode.FSDirectory: GROUP serial map: bits=24 maxEntries=16777215
2022-04-03 08:38:53,824 INFO namenode.FSDirectory: XATTR serial map: bits=24 maxEntries=16777215
2022-04-03 08:38:53,838 INFO util.GSet: Computing capacity for map INodeMap
2022-04-03 08:38:53,839 INFO util.GSet: VM type       = 64-bit
2022-04-03 08:38:53,839 INFO util.GSet: 1.0% max memory 452 MB = 4.5 MB
2022-04-03 08:38:53,839 INFO util.GSet: capacity      = 2^19 = 524288 entries
2022-04-03 08:38:53,846 INFO namenode.FSDirectory: ACLs enabled? true
2022-04-03 08:38:53,846 INFO namenode.FSDirectory: POSIX ACL inheritance enabled? true
2022-04-03 08:38:53,846 INFO namenode.FSDirectory: XAttrs enabled? true
2022-04-03 08:38:53,846 INFO namenode.NameNode: Caching file names occurring more than 10 times
2022-04-03 08:38:53,867 INFO snapshot.SnapshotManager: Loaded config captureOpenFiles: false, skipCaptureAccessTimeOnlyChange: false, snapshotDiffAllowSnapRootDescendant: true, maxSnapshotLimit: 65536
2022-04-03 08:38:53,892 INFO snapshot.SnapshotManager: SkipList is disabled
2022-04-03 08:38:53,901 INFO util.GSet: Computing capacity for map cachedBlocks
2022-04-03 08:38:53,901 INFO util.GSet: VM type       = 64-bit
2022-04-03 08:38:53,902 INFO util.GSet: 0.25% max memory 452 MB = 1.1 MB
2022-04-03 08:38:53,902 INFO util.GSet: capacity      = 2^17 = 131072 entries
2022-04-03 08:38:53,924 INFO metrics.TopMetrics: NNTop conf: dfs.namenode.top.window.num.buckets = 10
2022-04-03 08:38:53,924 INFO metrics.TopMetrics: NNTop conf: dfs.namenode.top.num.users = 10
2022-04-03 08:38:53,924 INFO metrics.TopMetrics: NNTop conf: dfs.namenode.top.windows.minutes = 1,5,25
2022-04-03 08:38:53,931 INFO namenode.FSNamesystem: Retry cache on namenode is enabled
2022-04-03 08:38:53,932 INFO namenode.FSNamesystem: Retry cache will use 0.03 of total heap and retry cache entry expiry time is 600000 millis
2022-04-03 08:38:53,934 INFO util.GSet: Computing capacity for map NameNodeRetryCache
2022-04-03 08:38:53,934 INFO util.GSet: VM type       = 64-bit
2022-04-03 08:38:53,934 INFO util.GSet: 0.029999999329447746% max memory 452 MB = 138.9 KB
2022-04-03 08:38:53,934 INFO util.GSet: capacity      = 2^14 = 16384 entries
2022-04-03 08:38:53,969 INFO namenode.FSImage: Allocated new BlockPoolId: BP-1684059263-192.168.121.134-1649000333955
2022-04-03 08:38:54,015 INFO common.Storage: Storage directory /opt/hadoop-3.3.2/tmpdata/dfs/name has been successfully formatted.
2022-04-03 08:38:54,080 INFO namenode.FSImageFormatProtobuf: Saving image file /opt/hadoop-3.3.2/tmpdata/dfs/name/current/fsimage.ckpt_0000000000000000000 using no compression
2022-04-03 08:38:54,251 INFO namenode.FSImageFormatProtobuf: Image file /opt/hadoop-3.3.2/tmpdata/dfs/name/current/fsimage.ckpt_0000000000000000000 of size 399 bytes saved in 0 seconds .
2022-04-03 08:38:54,296 INFO namenode.NNStorageRetentionManager: Going to retain 1 images with txid >= 0
2022-04-03 08:38:54,320 INFO namenode.FSNamesystem: Stopping services started for active state
2022-04-03 08:38:54,320 INFO namenode.FSNamesystem: Stopping services started for standby state
2022-04-03 08:38:54,330 INFO namenode.FSImage: FSImageSaver clean checkpoint: txid=0 when meet shutdown.
2022-04-03 08:38:54,331 INFO namenode.NameNode: SHUTDOWN_MSG: 
/************************************************************
SHUTDOWN_MSG: Shutting down NameNode at hadoop01/192.168.121.134
************************************************************/
[root@hadoop01 opt]# start-all.sh 
Starting namenodes on [hadoop01]
ERROR: Attempting to operate on hdfs namenode as root
ERROR: but there is no HDFS_NAMENODE_USER defined. Aborting operation.
Starting datanodes
ERROR: Attempting to operate on hdfs datanode as root
ERROR: but there is no HDFS_DATANODE_USER defined. Aborting operation.
Starting secondary namenodes [hadoop03]
ERROR: Attempting to operate on hdfs secondarynamenode as root
ERROR: but there is no HDFS_SECONDARYNAMENODE_USER defined. Aborting operation.
Starting resourcemanager
ERROR: Attempting to operate on yarn resourcemanager as root
ERROR: but there is no YARN_RESOURCEMANAGER_USER defined. Aborting operation.
Starting nodemanagers
ERROR: Attempting to operate on yarn nodemanager as root
ERROR: but there is no YARN_NODEMANAGER_USER defined. Aborting operation.
[root@hadoop01 opt]# jps
9927 Jps
7544 ResourceManager
7704 NodeManager
[root@hadoop01 opt]# cd ..
[root@hadoop01 /]# ll
total 28
lrwxrwxrwx.   1 root root    7 Aug 12  2018 bin -> usr/bin
dr-xr-xr-x.   5 root root 4096 Mar 26 23:54 boot
drwxr-xr-x    2 root root   26 Mar 27 02:32 c
drwxr-xr-x   19 root root 3260 Apr  3 08:07 dev
drwxr-xr-x. 140 root root 8192 Apr  3 08:29 etc
drwxr-xr-x    5 root root   50 Mar 27 02:50 export
drwxr-xr-x.   5 root root   44 Apr  3 07:12 home
lrwxrwxrwx.   1 root root    7 Aug 12  2018 lib -> usr/lib
lrwxrwxrwx.   1 root root    9 Aug 12  2018 lib64 -> usr/lib64
drwxr-xr-x.   2 root root    6 Aug 12  2018 media
drwxr-xr-x.   4 root root   31 Mar 27 00:14 mnt
drwxr-xr-x.   3 root root   80 Apr  3 06:51 opt
dr-xr-xr-x  283 root root    0 Apr  3 08:06 proc
dr-xr-x---.  18 root root 4096 Apr  3 08:35 root
drwxr-xr-x   40 root root 1200 Apr  3 08:07 run
lrwxrwxrwx.   1 root root    8 Aug 12  2018 sbin -> usr/sbin
drwxr-xr-x.   2 root root    6 Aug 12  2018 srv
dr-xr-xr-x   13 root root    0 Apr  3 08:06 sys
drwxrwxrwt.  46 root root 4096 Apr  3 08:38 tmp
drwxr-xr-x.  12 root root  144 Mar 26 23:47 usr
drwxr-xr-x.  22 root root 4096 Mar 27 00:31 var
drwxr-xr-x.   6 root root   79 Mar 27 00:31 www
[root@hadoop01 /]# cd /opt/hadoop-3.3.2/
[root@hadoop01 hadoop-3.3.2]# ll
total 88
drwxr-xr-x 2 root root   203 Apr  3 06:51 bin
drwxr-xr-x 3 root root    17 Apr  3 06:52 data
drwxr-xr-x 3 root root    20 Apr  3 06:52 etc
drwxr-xr-x 2 root root   106 Apr  3 06:51 include
drwxr-xr-x 3 root root    20 Apr  3 06:52 lib
drwxr-xr-x 4 root root   288 Apr  3 06:51 libexec
-rw-r--r-- 1 root root 23424 Apr  3 08:32 LICENSE-binary
drwxr-xr-x 2 root root  4096 Apr  3 06:51 licenses-binary
-rw-r--r-- 1 root root 15217 Apr  3 08:32 LICENSE.txt
drwxr-xr-x 2 root root    37 Apr  3 08:38 logs
-rw-r--r-- 1 root root 29473 Apr  3 08:32 NOTICE-binary
-rw-r--r-- 1 root root  1541 Apr  3 08:32 NOTICE.txt
-rw-r--r-- 1 root root   175 Apr  3 08:32 README.txt
drwxr-xr-x 3 root root  4096 Apr  3 06:51 sbin
drwxr-xr-x 4 root root    31 Apr  3 06:52 share
drwxr-xr-x 3 root root    17 Apr  3 08:38 tmpdata
[root@hadoop01 hadoop-3.3.2]# cd logs/
[root@hadoop01 logs]# ls
SecurityAuth-root.audit
[root@hadoop01 logs]# ll
total 0
-rw-r--r-- 1 root root 0 Apr  3 08:33 SecurityAuth-root.audit
[root@hadoop01 logs]# hdfs namenode -format
2022-04-03 08:40:04,946 INFO namenode.NameNode: STARTUP_MSG: 
/************************************************************
STARTUP_MSG: Starting NameNode
STARTUP_MSG:   host = hadoop01/192.168.121.134
STARTUP_MSG:   args = [-format]
STARTUP_MSG:   version = 3.3.2
STARTUP_MSG:   classpath = /opt/hadoop-3.3.2//etc/hadoop:/opt/hadoop-3.3.2//share/hadoop/common/lib/accessors-smart-2.4.7.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/animal-sniffer-annotations-1.17.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/asm-5.0.4.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/audience-annotations-0.5.0.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/avro-1.7.7.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/checker-qual-2.5.2.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/commons-beanutils-1.9.4.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/commons-cli-1.2.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/commons-codec-1.11.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/commons-collections-3.2.2.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/commons-compress-1.21.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/commons-configuration2-2.1.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/commons-daemon-1.0.13.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/commons-io-2.8.0.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/commons-lang3-3.12.0.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/commons-logging-1.1.3.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/commons-math3-3.1.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/commons-net-3.6.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/commons-text-1.4.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/curator-client-4.2.0.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/curator-framework-4.2.0.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/curator-recipes-4.2.0.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/dnsjava-2.1.7.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/failureaccess-1.0.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/gson-2.8.9.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/guava-27.0-jre.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/hadoop-annotations-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/hadoop-auth-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/hadoop-shaded-guava-1.1.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/hadoop-shaded-protobuf_3_7-1.1.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/httpclient-4.5.13.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/httpcore-4.4.13.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/j2objc-annotations-1.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jackson-annotations-2.13.0.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jackson-core-2.13.0.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jackson-core-asl-1.9.13.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jackson-databind-2.13.0.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jackson-jaxrs-1.9.13.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jackson-mapper-asl-1.9.13.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jackson-xc-1.9.13.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jakarta.activation-api-1.2.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/javax.servlet-api-3.1.0.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jaxb-api-2.2.11.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jaxb-impl-2.2.3-1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jcip-annotations-1.0-1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jersey-core-1.19.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jersey-json-1.19.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jersey-server-1.19.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jersey-servlet-1.19.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jettison-1.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jetty-http-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jetty-io-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jetty-security-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jetty-server-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jetty-servlet-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jetty-util-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jetty-util-ajax-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jetty-webapp-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jetty-xml-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jsch-0.1.55.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/json-smart-2.4.7.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jsp-api-2.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jsr305-3.0.2.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jsr311-api-1.1.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/jul-to-slf4j-1.7.30.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerb-admin-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerb-client-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerb-common-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerb-core-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerb-crypto-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerb-identity-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerb-server-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerb-simplekdc-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerb-util-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerby-asn1-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerby-config-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerby-pkix-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerby-util-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/kerby-xdr-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/listenablefuture-9999.0-empty-to-avoid-conflict-with-guava.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/log4j-1.2.17.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/metrics-core-3.2.4.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/netty-3.10.6.Final.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/nimbus-jose-jwt-9.8.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/paranamer-2.3.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/protobuf-java-2.5.0.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/re2j-1.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/slf4j-api-1.7.30.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/slf4j-log4j12-1.7.30.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/snappy-java-1.1.8.2.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/stax2-api-4.2.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/token-provider-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/woodstox-core-5.3.0.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/zookeeper-3.5.6.jar:/opt/hadoop-3.3.2//share/hadoop/common/lib/zookeeper-jute-3.5.6.jar:/opt/hadoop-3.3.2//share/hadoop/common/hadoop-common-3.3.2-tests.jar:/opt/hadoop-3.3.2//share/hadoop/common/hadoop-common-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/common/hadoop-kms-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/common/hadoop-nfs-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/common/hadoop-registry-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/accessors-smart-2.4.7.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/animal-sniffer-annotations-1.17.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/asm-5.0.4.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/audience-annotations-0.5.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/avro-1.7.7.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/checker-qual-2.5.2.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/commons-beanutils-1.9.4.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/commons-cli-1.2.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/commons-codec-1.11.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/commons-collections-3.2.2.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/commons-compress-1.21.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/commons-configuration2-2.1.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/commons-daemon-1.0.13.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/commons-io-2.8.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/commons-lang3-3.12.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/commons-logging-1.1.3.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/commons-math3-3.1.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/commons-net-3.6.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/commons-text-1.4.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/curator-client-4.2.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/curator-framework-4.2.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/curator-recipes-4.2.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/dnsjava-2.1.7.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/failureaccess-1.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/gson-2.8.9.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/guava-27.0-jre.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/hadoop-annotations-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/hadoop-auth-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/hadoop-shaded-guava-1.1.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/hadoop-shaded-protobuf_3_7-1.1.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/httpclient-4.5.13.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/httpcore-4.4.13.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/j2objc-annotations-1.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jackson-annotations-2.13.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jackson-core-2.13.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jackson-core-asl-1.9.13.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jackson-databind-2.13.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jackson-jaxrs-1.9.13.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jackson-mapper-asl-1.9.13.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jackson-xc-1.9.13.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jakarta.activation-api-1.2.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/javax.servlet-api-3.1.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jaxb-api-2.2.11.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jaxb-impl-2.2.3-1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jcip-annotations-1.0-1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jersey-core-1.19.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jersey-json-1.19.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jersey-server-1.19.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jersey-servlet-1.19.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jettison-1.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jetty-http-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jetty-io-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jetty-security-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jetty-server-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jetty-servlet-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jetty-util-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jetty-util-ajax-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jetty-webapp-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jetty-xml-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jsch-0.1.55.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/json-simple-1.1.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/json-smart-2.4.7.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jsr305-3.0.2.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/jsr311-api-1.1.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerb-admin-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerb-client-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerb-common-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerb-core-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerb-crypto-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerb-identity-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerb-server-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerb-simplekdc-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerb-util-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerby-asn1-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerby-config-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerby-pkix-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerby-util-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/kerby-xdr-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/leveldbjni-all-1.8.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/listenablefuture-9999.0-empty-to-avoid-conflict-with-guava.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/log4j-1.2.17.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/netty-3.10.6.Final.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/netty-all-4.1.68.Final.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/nimbus-jose-jwt-9.8.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/okhttp-2.7.5.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/okio-1.6.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/paranamer-2.3.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/protobuf-java-2.5.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/re2j-1.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/snappy-java-1.1.8.2.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/stax2-api-4.2.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/token-provider-1.0.1.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/woodstox-core-5.3.0.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/zookeeper-3.5.6.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/lib/zookeeper-jute-3.5.6.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/hadoop-hdfs-3.3.2-tests.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/hadoop-hdfs-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/hadoop-hdfs-client-3.3.2-tests.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/hadoop-hdfs-client-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/hadoop-hdfs-httpfs-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/hadoop-hdfs-native-client-3.3.2-tests.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/hadoop-hdfs-native-client-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/hadoop-hdfs-nfs-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/hadoop-hdfs-rbf-3.3.2-tests.jar:/opt/hadoop-3.3.2//share/hadoop/hdfs/hadoop-hdfs-rbf-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/mapreduce/hadoop-mapreduce-client-app-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/mapreduce/hadoop-mapreduce-client-common-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/mapreduce/hadoop-mapreduce-client-core-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/mapreduce/hadoop-mapreduce-client-hs-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/mapreduce/hadoop-mapreduce-client-hs-plugins-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/mapreduce/hadoop-mapreduce-client-jobclient-3.3.2-tests.jar:/opt/hadoop-3.3.2//share/hadoop/mapreduce/hadoop-mapreduce-client-jobclient-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/mapreduce/hadoop-mapreduce-client-nativetask-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/mapreduce/hadoop-mapreduce-client-shuffle-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/mapreduce/hadoop-mapreduce-client-uploader-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/mapreduce/hadoop-mapreduce-examples-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/HikariCP-java7-2.4.12.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/aopalliance-1.0.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/asm-analysis-9.1.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/asm-commons-9.1.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/asm-tree-9.1.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/bcpkix-jdk15on-1.60.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/bcprov-jdk15on-1.60.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/ehcache-3.3.1.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/fst-2.50.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/geronimo-jcache_1.0_spec-1.0-alpha-1.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/guice-4.0.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/guice-servlet-4.0.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/jackson-jaxrs-base-2.13.0.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/jackson-jaxrs-json-provider-2.13.0.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/jackson-module-jaxb-annotations-2.13.0.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/jakarta.xml.bind-api-2.3.3.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/java-util-1.9.0.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/javax-websocket-client-impl-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/javax-websocket-server-impl-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/javax.inject-1.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/javax.websocket-api-1.0.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/javax.websocket-client-api-1.0.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/javax.ws.rs-api-2.1.1.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/jersey-client-1.19.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/jersey-guice-1.19.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/jetty-annotations-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/jetty-client-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/jetty-jndi-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/jetty-plus-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/jline-3.9.0.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/jna-5.2.0.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/json-io-2.5.1.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/metrics-core-3.2.4.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/mssql-jdbc-6.2.1.jre7.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/objenesis-2.6.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/snakeyaml-1.26.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/swagger-annotations-1.5.4.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/websocket-api-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/websocket-client-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/websocket-common-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/websocket-server-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/lib/websocket-servlet-9.4.43.v20210629.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-api-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-applications-distributedshell-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-applications-mawo-core-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-applications-unmanaged-am-launcher-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-client-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-common-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-registry-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-server-applicationhistoryservice-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-server-common-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-server-nodemanager-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-server-resourcemanager-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-server-router-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-server-sharedcachemanager-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-server-tests-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-server-timeline-pluginstorage-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-server-web-proxy-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-services-api-3.3.2.jar:/opt/hadoop-3.3.2//share/hadoop/yarn/hadoop-yarn-services-core-3.3.2.jar
STARTUP_MSG:   build = git@github.com:apache/hadoop.git -r 0bcb014209e219273cb6fd4152df7df713cbac61; compiled by 'chao' on 2022-02-21T18:39Z
STARTUP_MSG:   java = 11.0.1
************************************************************/
2022-04-03 08:40:04,958 INFO namenode.NameNode: registered UNIX signal handlers for [TERM, HUP, INT]
2022-04-03 08:40:05,090 INFO namenode.NameNode: createNameNode [-format]
2022-04-03 08:40:05,751 INFO namenode.NameNode: Formatting using clusterid: CID-68262871-f907-4ac0-a2b0-e6ef32574479
2022-04-03 08:40:05,821 INFO namenode.FSEditLog: Edit logging is async:true
2022-04-03 08:40:05,867 INFO namenode.FSNamesystem: KeyProvider: null
2022-04-03 08:40:05,869 INFO namenode.FSNamesystem: fsLock is fair: true
2022-04-03 08:40:05,869 INFO namenode.FSNamesystem: Detailed lock hold time metrics enabled: false
2022-04-03 08:40:05,927 INFO namenode.FSNamesystem: fsOwner                = root (auth:SIMPLE)
2022-04-03 08:40:05,927 INFO namenode.FSNamesystem: supergroup             = supergroup
2022-04-03 08:40:05,927 INFO namenode.FSNamesystem: isPermissionEnabled    = true
2022-04-03 08:40:05,927 INFO namenode.FSNamesystem: isStoragePolicyEnabled = true
2022-04-03 08:40:05,927 INFO namenode.FSNamesystem: HA Enabled: false
2022-04-03 08:40:06,009 INFO common.Util: dfs.datanode.fileio.profiling.sampling.percentage set to 0. Disabling file IO profiling
2022-04-03 08:40:06,020 INFO blockmanagement.DatanodeManager: dfs.block.invalidate.limit: configured=1000, counted=60, effected=1000
2022-04-03 08:40:06,020 INFO blockmanagement.DatanodeManager: dfs.namenode.datanode.registration.ip-hostname-check=true
2022-04-03 08:40:06,024 INFO blockmanagement.BlockManager: dfs.namenode.startup.delay.block.deletion.sec is set to 000:00:00:00.000
2022-04-03 08:40:06,024 INFO blockmanagement.BlockManager: The block deletion will start around 2022 Apr 03 08:40:06
2022-04-03 08:40:06,026 INFO util.GSet: Computing capacity for map BlocksMap
2022-04-03 08:40:06,026 INFO util.GSet: VM type       = 64-bit
2022-04-03 08:40:06,027 INFO util.GSet: 2.0% max memory 452 MB = 9.0 MB
2022-04-03 08:40:06,027 INFO util.GSet: capacity      = 2^20 = 1048576 entries
2022-04-03 08:40:06,038 INFO blockmanagement.BlockManager: Storage policy satisfier is disabled
2022-04-03 08:40:06,038 INFO blockmanagement.BlockManager: dfs.block.access.token.enable = false
2022-04-03 08:40:06,047 INFO blockmanagement.BlockManagerSafeMode: dfs.namenode.safemode.threshold-pct = 0.999
2022-04-03 08:40:06,047 INFO blockmanagement.BlockManagerSafeMode: dfs.namenode.safemode.min.datanodes = 0
2022-04-03 08:40:06,047 INFO blockmanagement.BlockManagerSafeMode: dfs.namenode.safemode.extension = 30000
2022-04-03 08:40:06,048 INFO blockmanagement.BlockManager: defaultReplication         = 3
2022-04-03 08:40:06,048 INFO blockmanagement.BlockManager: maxReplication             = 512
2022-04-03 08:40:06,048 INFO blockmanagement.BlockManager: minReplication             = 1
2022-04-03 08:40:06,048 INFO blockmanagement.BlockManager: maxReplicationStreams      = 2
2022-04-03 08:40:06,048 INFO blockmanagement.BlockManager: redundancyRecheckInterval  = 3000ms
2022-04-03 08:40:06,048 INFO blockmanagement.BlockManager: encryptDataTransfer        = false
2022-04-03 08:40:06,048 INFO blockmanagement.BlockManager: maxNumBlocksToLog          = 1000
2022-04-03 08:40:06,072 INFO namenode.FSDirectory: GLOBAL serial map: bits=29 maxEntries=536870911
2022-04-03 08:40:06,072 INFO namenode.FSDirectory: USER serial map: bits=24 maxEntries=16777215
2022-04-03 08:40:06,072 INFO namenode.FSDirectory: GROUP serial map: bits=24 maxEntries=16777215
2022-04-03 08:40:06,073 INFO namenode.FSDirectory: XATTR serial map: bits=24 maxEntries=16777215
2022-04-03 08:40:06,109 INFO util.GSet: Computing capacity for map INodeMap
2022-04-03 08:40:06,109 INFO util.GSet: VM type       = 64-bit
2022-04-03 08:40:06,109 INFO util.GSet: 1.0% max memory 452 MB = 4.5 MB
2022-04-03 08:40:06,109 INFO util.GSet: capacity      = 2^19 = 524288 entries
2022-04-03 08:40:06,110 INFO namenode.FSDirectory: ACLs enabled? true
2022-04-03 08:40:06,110 INFO namenode.FSDirectory: POSIX ACL inheritance enabled? true
2022-04-03 08:40:06,111 INFO namenode.FSDirectory: XAttrs enabled? true
2022-04-03 08:40:06,111 INFO namenode.NameNode: Caching file names occurring more than 10 times
2022-04-03 08:40:06,124 INFO snapshot.SnapshotManager: Loaded config captureOpenFiles: false, skipCaptureAccessTimeOnlyChange: false, snapshotDiffAllowSnapRootDescendant: true, maxSnapshotLimit: 65536
2022-04-03 08:40:06,126 INFO snapshot.SnapshotManager: SkipList is disabled
2022-04-03 08:40:06,132 INFO util.GSet: Computing capacity for map cachedBlocks
2022-04-03 08:40:06,132 INFO util.GSet: VM type       = 64-bit
2022-04-03 08:40:06,132 INFO util.GSet: 0.25% max memory 452 MB = 1.1 MB
2022-04-03 08:40:06,132 INFO util.GSet: capacity      = 2^17 = 131072 entries
2022-04-03 08:40:06,141 INFO metrics.TopMetrics: NNTop conf: dfs.namenode.top.window.num.buckets = 10
2022-04-03 08:40:06,141 INFO metrics.TopMetrics: NNTop conf: dfs.namenode.top.num.users = 10
2022-04-03 08:40:06,141 INFO metrics.TopMetrics: NNTop conf: dfs.namenode.top.windows.minutes = 1,5,25
2022-04-03 08:40:06,149 INFO namenode.FSNamesystem: Retry cache on namenode is enabled
2022-04-03 08:40:06,149 INFO namenode.FSNamesystem: Retry cache will use 0.03 of total heap and retry cache entry expiry time is 600000 millis
2022-04-03 08:40:06,150 INFO util.GSet: Computing capacity for map NameNodeRetryCache
2022-04-03 08:40:06,150 INFO util.GSet: VM type       = 64-bit
2022-04-03 08:40:06,150 INFO util.GSet: 0.029999999329447746% max memory 452 MB = 138.9 KB
2022-04-03 08:40:06,150 INFO util.GSet: capacity      = 2^14 = 16384 entries
Re-format filesystem in Storage Directory root= /opt/hadoop-3.3.2/tmpdata/dfs/name; location= null ? (Y or N) Y
2022-04-03 08:40:10,387 INFO namenode.FSImage: Allocated new BlockPoolId: BP-1829021315-192.168.121.134-1649000410379
2022-04-03 08:40:10,387 INFO common.Storage: Will remove files: [/opt/hadoop-3.3.2/tmpdata/dfs/name/current/VERSION, /opt/hadoop-3.3.2/tmpdata/dfs/name/current/seen_txid, /opt/hadoop-3.3.2/tmpdata/dfs/name/current/fsimage_0000000000000000000.md5, /opt/hadoop-3.3.2/tmpdata/dfs/name/current/fsimage_0000000000000000000]
2022-04-03 08:40:10,404 INFO common.Storage: Storage directory /opt/hadoop-3.3.2/tmpdata/dfs/name has been successfully formatted.
2022-04-03 08:40:10,459 INFO namenode.FSImageFormatProtobuf: Saving image file /opt/hadoop-3.3.2/tmpdata/dfs/name/current/fsimage.ckpt_0000000000000000000 using no compression
2022-04-03 08:40:10,574 INFO namenode.FSImageFormatProtobuf: Image file /opt/hadoop-3.3.2/tmpdata/dfs/name/current/fsimage.ckpt_0000000000000000000 of size 399 bytes saved in 0 seconds .
2022-04-03 08:40:10,589 INFO namenode.NNStorageRetentionManager: Going to retain 1 images with txid >= 0
2022-04-03 08:40:10,621 INFO namenode.FSNamesystem: Stopping services started for active state
2022-04-03 08:40:10,622 INFO namenode.FSNamesystem: Stopping services started for standby state
2022-04-03 08:40:10,631 INFO namenode.FSImage: FSImageSaver clean checkpoint: txid=0 when meet shutdown.
2022-04-03 08:40:10,632 INFO namenode.NameNode: SHUTDOWN_MSG: 
/************************************************************
SHUTDOWN_MSG: Shutting down NameNode at hadoop01/192.168.121.134
************************************************************/
[root@hadoop01 logs]# jps
7544 ResourceManager
7704 NodeManager
10028 Jps
[root@hadoop01 logs]# kill - 9 7544 7704
-bash: kill: : invalid signal specification
[root@hadoop01 logs]# jps
7544 ResourceManager
7704 NodeManager
10046 Jps
[root@hadoop01 logs]# kill -9 7544 7704
[root@hadoop01 logs]# 
[root@hadoop01 logs]# jps
10072 Jps
[root@hadoop01 logs]# start-dfs.sh 
Starting namenodes on [hadoop01]
ERROR: Attempting to operate on hdfs namenode as root
ERROR: but there is no HDFS_NAMENODE_USER defined. Aborting operation.
Starting datanodes
ERROR: Attempting to operate on hdfs datanode as root
ERROR: but there is no HDFS_DATANODE_USER defined. Aborting operation.
Starting secondary namenodes [hadoop03]
ERROR: Attempting to operate on hdfs secondarynamenode as root
ERROR: but there is no HDFS_SECONDARYNAMENODE_USER defined. Aborting operation.
[root@hadoop01 logs]# jps
10322 Jps
[root@hadoop01 logs]# cd ..
[root@hadoop01 hadoop-3.3.2]# cd ..
[root@hadoop01 opt]# cd hadoop-3.3.2/logs/
[root@hadoop01 logs]# ll
total 0
-rw-r--r-- 1 root root 0 Apr  3 08:33 SecurityAuth-root.audit
[root@hadoop01 logs]# cd ..
[root@hadoop01 hadoop-3.3.2]# ssh hadoop02
Activate the web console with: systemctl enable --now cockpit.socket

Last login: Sun Apr  3 08:07:37 2022 from 192.168.121.5
[root@hadoop02 ~]# exit
logout
Connection to hadoop02 closed.
[root@hadoop01 hadoop-3.3.2]# ls
bin   etc      lib      LICENSE-binary   LICENSE.txt  NOTICE-binary  README.txt  share
data  include  libexec  licenses-binary  logs         NOTICE.txt     sbin        tmpdata
[root@hadoop01 hadoop-3.3.2]# ll
total 88
drwxr-xr-x 2 root root   203 Apr  3 06:51 bin
drwxr-xr-x 3 root root    17 Apr  3 06:52 data
drwxr-xr-x 3 root root    20 Apr  3 06:52 etc
drwxr-xr-x 2 root root   106 Apr  3 06:51 include
drwxr-xr-x 3 root root    20 Apr  3 06:52 lib
drwxr-xr-x 4 root root   288 Apr  3 06:51 libexec
-rw-r--r-- 1 root root 23424 Apr  3 08:32 LICENSE-binary
drwxr-xr-x 2 root root  4096 Apr  3 06:51 licenses-binary
-rw-r--r-- 1 root root 15217 Apr  3 08:32 LICENSE.txt
drwxr-xr-x 2 root root    37 Apr  3 08:40 logs
-rw-r--r-- 1 root root 29473 Apr  3 08:32 NOTICE-binary
-rw-r--r-- 1 root root  1541 Apr  3 08:32 NOTICE.txt
-rw-r--r-- 1 root root   175 Apr  3 08:32 README.txt
drwxr-xr-x 3 root root  4096 Apr  3 06:51 sbin
drwxr-xr-x 4 root root    31 Apr  3 06:52 share
drwxr-xr-x 3 root root    17 Apr  3 08:38 tmpdata
[root@hadoop01 hadoop-3.3.2]# ls
bin   etc      lib      LICENSE-binary   LICENSE.txt  NOTICE-binary  README.txt  share
data  include  libexec  licenses-binary  logs         NOTICE.txt     sbin        tmpdata
[root@hadoop01 hadoop-3.3.2]# rm -rf data/
[root@hadoop01 hadoop-3.3.2]# ls
bin  include  libexec         licenses-binary  logs           NOTICE.txt  sbin   tmpdata
etc  lib      LICENSE-binary  LICENSE.txt      NOTICE-binary  README.txt  share
[root@hadoop01 hadoop-3.3.2]# ll
total 88
drwxr-xr-x 2 root root   203 Apr  3 06:51 bin
drwxr-xr-x 3 root root    20 Apr  3 06:52 etc
drwxr-xr-x 2 root root   106 Apr  3 06:51 include
drwxr-xr-x 3 root root    20 Apr  3 06:52 lib
drwxr-xr-x 4 root root   288 Apr  3 06:51 libexec
-rw-r--r-- 1 root root 23424 Apr  3 08:32 LICENSE-binary
drwxr-xr-x 2 root root  4096 Apr  3 06:51 licenses-binary
-rw-r--r-- 1 root root 15217 Apr  3 08:32 LICENSE.txt
drwxr-xr-x 2 root root    37 Apr  3 08:40 logs
-rw-r--r-- 1 root root 29473 Apr  3 08:32 NOTICE-binary
-rw-r--r-- 1 root root  1541 Apr  3 08:32 NOTICE.txt
-rw-r--r-- 1 root root   175 Apr  3 08:32 README.txt
drwxr-xr-x 3 root root  4096 Apr  3 06:51 sbin
drwxr-xr-x 4 root root    31 Apr  3 06:52 share
drwxr-xr-x 3 root root    17 Apr  3 08:38 tmpdata
[root@hadoop01 hadoop-3.3.2]# rm -rf logs/
[root@hadoop01 hadoop-3.3.2]# 
[root@hadoop01 hadoop-3.3.2]# rm -rf logs/
[root@hadoop01 hadoop-3.3.2]# ll
total 88
drwxr-xr-x 2 root root   203 Apr  3 06:51 bin
drwxr-xr-x 3 root root    20 Apr  3 06:52 etc
drwxr-xr-x 2 root root   106 Apr  3 06:51 include
drwxr-xr-x 3 root root    20 Apr  3 06:52 lib
drwxr-xr-x 4 root root   288 Apr  3 06:51 libexec
-rw-r--r-- 1 root root 23424 Apr  3 08:32 LICENSE-binary
drwxr-xr-x 2 root root  4096 Apr  3 06:51 licenses-binary
-rw-r--r-- 1 root root 15217 Apr  3 08:32 LICENSE.txt
-rw-r--r-- 1 root root 29473 Apr  3 08:32 NOTICE-binary
-rw-r--r-- 1 root root  1541 Apr  3 08:32 NOTICE.txt
-rw-r--r-- 1 root root   175 Apr  3 08:32 README.txt
drwxr-xr-x 3 root root  4096 Apr  3 06:51 sbin
drwxr-xr-x 4 root root    31 Apr  3 06:52 share
drwxr-xr-x 3 root root    17 Apr  3 08:38 tmpdata
[root@hadoop01 hadoop-3.3.2]# bin/
container-executor       hdfs.cmd                 test-container-executor
hadoop                   mapred                   yarn
hadoop.cmd               mapred.cmd               yarn.cmd
hdfs                     oom-listener             
[root@hadoop01 hadoop-3.3.2]# bin/hadoop
hadoop      hadoop.cmd  
[root@hadoop01 hadoop-3.3.2]# sbin/
distribute-exclude.sh    start-all.sh             stop-balancer.sh
FederationStateStore/    start-balancer.sh        stop-dfs.cmd
hadoop-daemon.sh         start-dfs.cmd            stop-dfs.sh
hadoop-daemons.sh        start-dfs.sh             stop-secure-dns.sh
httpfs.sh                start-secure-dns.sh      stop-yarn.cmd
kms.sh                   start-yarn.cmd           stop-yarn.sh
mr-jobhistory-daemon.sh  start-yarn.sh            workers.sh
refresh-namenodes.sh     stop-all.cmd             yarn-daemon.sh
start-all.cmd            stop-all.sh              yarn-daemons.sh
[root@hadoop01 hadoop-3.3.2]# sbin/hadoop-daemon.sh start namenode
WARNING: Use of this script to start HDFS daemons is deprecated.
WARNING: Attempting to execute replacement "hdfs --daemon start" instead.
WARNING: /opt/hadoop-3.3.2//logs does not exist. Creating.
[root@hadoop01 hadoop-3.3.2]# jps
10518 Jps
10445 NameNode
[root@hadoop01 hadoop-3.3.2]# start-all.sh 
Starting namenodes on [hadoop01]
ERROR: Attempting to operate on hdfs namenode as root
ERROR: but there is no HDFS_NAMENODE_USER defined. Aborting operation.
Starting datanodes
ERROR: Attempting to operate on hdfs datanode as root
ERROR: but there is no HDFS_DATANODE_USER defined. Aborting operation.
Starting secondary namenodes [hadoop03]
ERROR: Attempting to operate on hdfs secondarynamenode as root
ERROR: but there is no HDFS_SECONDARYNAMENODE_USER defined. Aborting operation.
Starting resourcemanager
ERROR: Attempting to operate on yarn resourcemanager as root
ERROR: but there is no YARN_RESOURCEMANAGER_USER defined. Aborting operation.
Starting nodemanagers
ERROR: Attempting to operate on yarn nodemanager as root
ERROR: but there is no YARN_NODEMANAGER_USER defined. Aborting operation.
[root@hadoop01 hadoop-3.3.2]# jps
10918 Jps
10445 NameNode
[root@hadoop01 hadoop-3.3.2]# hadoop-daemon.sh start datanode
WARNING: Use of this script to start HDFS daemons is deprecated.
WARNING: Attempting to execute replacement "hdfs --daemon start" instead.
[root@hadoop01 hadoop-3.3.2]# jps
10994 DataNode
11032 Jps
10445 NameNode
[root@hadoop01 hadoop-3.3.2]# start-yarn.sh 
Starting resourcemanager
Last login: Sun Apr  3 08:35:40 PDT 2022 from 192.168.121.5 on pts/2
Starting nodemanagers
Last login: Sun Apr  3 08:44:02 PDT 2022 on pts/2
hadoop02: nodemanager is running as process 2756.  Stop it first and ensure /tmp/hadoop-root-nodemanager.pid file is empty before retry.
hadoop03: nodemanager is running as process 7589.  Stop it first and ensure /tmp/hadoop-root-nodemanager.pid file is empty before retry.
[root@hadoop01 hadoop-3.3.2]# jps
10994 DataNode
11223 ResourceManager
11736 Jps
11387 NodeManager
10445 NameNode
[root@hadoop01 hadoop-3.3.2]# jps
10994 DataNode
11223 ResourceManager
11754 Jps
11387 NodeManager
10445 NameNode
[root@hadoop01 hadoop-3.3.2]# cd etc/hadoop/
[root@hadoop01 hadoop]# ll
total 176
-rw-r--r-- 1 root root  9213 Apr  3 08:33 capacity-scheduler.xml
-rw-r--r-- 1 root root  1335 Apr  3 08:33 configuration.xsl
-rw-r--r-- 1 root root  2567 Apr  3 08:33 container-executor.cfg
-rw-r--r-- 1 root root   431 Apr  3 08:33 core-site.xml
-rw-r--r-- 1 root root  3999 Apr  3 08:33 hadoop-env.cmd
-rw-r--r-- 1 root root 16640 Apr  3 08:33 hadoop-env.sh
-rw-r--r-- 1 root root  3321 Apr  3 08:33 hadoop-metrics2.properties
-rw-r--r-- 1 root root 11765 Apr  3 08:33 hadoop-policy.xml
-rw-r--r-- 1 root root  3414 Apr  3 08:33 hadoop-user-functions.sh.example
-rw-r--r-- 1 root root   683 Apr  3 08:33 hdfs-rbf-site.xml
-rw-r--r-- 1 root root   442 Apr  3 08:33 hdfs-site.xml
-rw-r--r-- 1 root root  1484 Apr  3 08:33 httpfs-env.sh
-rw-r--r-- 1 root root  1657 Apr  3 08:33 httpfs-log4j.properties
-rw-r--r-- 1 root root   620 Apr  3 08:33 httpfs-site.xml
-rw-r--r-- 1 root root  3518 Apr  3 08:33 kms-acls.xml
-rw-r--r-- 1 root root  1351 Apr  3 08:33 kms-env.sh
-rw-r--r-- 1 root root  1860 Apr  3 08:33 kms-log4j.properties
-rw-r--r-- 1 root root   682 Apr  3 08:33 kms-site.xml
-rw-r--r-- 1 root root 13700 Apr  3 08:33 log4j.properties
-rw-r--r-- 1 root root   951 Apr  3 08:33 mapred-env.cmd
-rw-r--r-- 1 root root  1764 Apr  3 08:33 mapred-env.sh
-rw-r--r-- 1 root root  4113 Apr  3 08:33 mapred-queues.xml.template
-rw-r--r-- 1 root root   437 Apr  3 08:33 mapred-site.xml
drwxr-xr-x 2 root root    24 Apr  3 06:52 shellprofile.d
-rw-r--r-- 1 root root  2316 Apr  3 08:33 ssl-client.xml.example
-rw-r--r-- 1 root root  2697 Apr  3 08:33 ssl-server.xml.example
-rw-r--r-- 1 root root  2681 Apr  3 08:33 user_ec_policies.xml.template
-rw-r--r-- 1 root root    27 Apr  3 08:33 workers
-rw-r--r-- 1 root root  2250 Apr  3 08:33 yarn-env.cmd
-rw-r--r-- 1 root root  6329 Apr  3 08:33 yarn-env.sh
-rw-r--r-- 1 root root  2591 Apr  3 08:33 yarnservice-log4j.properties
-rw-r--r-- 1 root root   533 Apr  3 08:33 yarn-site.xml
[root@hadoop01 hadoop]# vi hdfs-site.xml 
[root@hadoop01 hadoop]# pwd
/opt/hadoop-3.3.2/etc/hadoop
[root@hadoop01 hadoop]# cd /export/servers/
[root@hadoop01 servers]# ls
hadoop-3.3.2         jdk                              jdk-8u161-linux-x64.tar.tmp
hadoop-3.3.2.tar.gz  jdk-11.0.1_linux-x64_bin.tar.gz
[root@hadoop01 servers]# vim ~/.bash
.bash_history  .bash_logout   .bash_profile  .bashrc        
[root@hadoop01 servers]# vim ~/.bash
.bash_history  .bash_logout   .bash_profile  .bashrc        
[root@hadoop01 servers]# vim ~/.bashrc 
[root@hadoop01 servers]# vim /etc/profile.d/my_path.sh 
[root@hadoop01 servers]# lsc
bash: lsc: command not found...
Failed to search for file: Cannot update read-only repo
[root@hadoop01 servers]# cd /opt/hadoop-3.3.2/etc/hadoop
[root@hadoop01 hadoop]# ls
capacity-scheduler.xml            httpfs-env.sh               mapred-site.xml
configuration.xsl                 httpfs-log4j.properties     shellprofile.d
container-executor.cfg            httpfs-site.xml             ssl-client.xml.example
core-site.xml                     kms-acls.xml                ssl-server.xml.example
hadoop-env.cmd                    kms-env.sh                  user_ec_policies.xml.template
hadoop-env.sh                     kms-log4j.properties        workers
hadoop-metrics2.properties        kms-site.xml                yarn-env.cmd
hadoop-policy.xml                 log4j.properties            yarn-env.sh
hadoop-user-functions.sh.example  mapred-env.cmd              yarnservice-log4j.properties
hdfs-rbf-site.xml                 mapred-env.sh               yarn-site.xml
hdfs-site.xml                     mapred-queues.xml.template
[root@hadoop01 hadoop]# vim hdfs-site.xml 

<?xml version="1.0" encoding="UTF-8"?>
<?xml-stylesheet type="text/xsl" href="configuration.xsl"?>
<configuration>
    <!-- nn web端访问地址-->
    <property>
        <name>dfs.namenode.http-address</name>
        <value>hadoop01:9870</value>
    </property>
<?xml version="1.0" encoding="UTF-8"?>
Socket error Event: 32 Error: 10053.f="configuration.xsl"?>
Connection closing...Socket close.
    <!-- nn web端访问地址-->
Connection closed by foreign host.
        <name>dfs.namenode.http-address</name>
Disconnected from remote host(hadoop01) at 23:54:28.
    </property>
Type `help' to learn how to use Xshell prompt.
[D:\~]$ 
Reconnecting in 60 seconds. Press any key to exit local shell.
......  <value>hadoop03:9868</value>
[D:\~]$ dddd:wq
</configuration>

```

