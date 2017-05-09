ZooKeeper Usage Demo
====================
Monitors a znode status in ZooKeeper and start/stop an external process, meanwhile record the znode value in a specified file.

### Usage
#### 1. Run ZooKeeper docker
`docker run -p 2181:2181 --name some-zookeeper --restart always -d zookeeper`

#### 2. Run the demo program
`java -jar target/zkdemo-1.0-jar-with-dependencies.jar 192.168.33.20:2181 /zkcluster-master /tmp/zkcluster java -jar /Users/yincaihua/github.com/caihua-yin/zkcluster/target/zkcluster-1.0.jar`

Reference:
https://zookeeper.apache.org/doc/trunk/javaExample.html
