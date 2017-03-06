## Hadoop完全分布式环境参数

Hadoop版本1.1.2

hosts
-----

# ============ Hadoop节点参数 =========

127.0.0.1 		Master.Hadoop // 每个节点均需修改
192.168.3.145   Slave1.Hadoop
192.168.3.146   Slave2.Hadoop
192.168.3.148   Master.Hadoop

# ============== END =================

jdk
-----
Master.Hadoop macOS 		jdk1.7 64bit
Slave1.Hadoop Ubuntu14.04   jdk1.7 64bit
Slave2.Hadoop Ubuntu14.04   jdk1.7 64bit

Slave结点设置
-----------
export HADOOP_HOME_WARN_SUPPRESS=0 
export JAVA_HOME=/usr/local/jdk1.7.0_25 
export CLASSPATH=.:$JAVA_HOME/lib/tools.jar:$JAVA_HOME/lib/dt.jar 
export PATH=$JAVA_HOME/bin:$PATH 
export HADOOP_HOME=/usr/local/hadoop 
export PATH=$HADOOP_HOME/bin:$PATH

## HBase完全分布式环境参数

HBase版本0.94.8
