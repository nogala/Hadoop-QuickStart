# Hadoop-QuickStart
Maven libraries from Hadoop
Install Hadoop instructions:
$ sudo su -
$ chkconfig iptables off; service iptables stop
$ nano /etc/selinux/config and change selinux=disabled
$ nano /etc/resolv.conf points to nameserver
$ useradd hadoop
$ su - hadoop
$ tar -xzvf hadoop-2.9.1.tar.gz 
$ sudo su -
$ mv hadoop-2.9.1 /opt/.
$ cd /opt
$ ln -s hadoop-2.7.3 hadoop
Setup ".bash_profile"
Hadoop Configuration files:
  core-site.xml
  hdfs-site.xml
  mapred-site.xml
  yarn-site.xml
Commands to start services:
$ hadoop namenode -format
$ hadoop-daemon.sh start namenode
$ hadoop-daemon.sh start datanode
$ yarn-daemon.sh start resourcemanager
$ yarn-daemon.sh start nodemanager
# Hadoop-QuickStart

Maven libraries from Hadoop

## Install Hadoop instructions:

`$ sudo su -`

`$ chkconfig iptables off; service iptables stop`

`$ nano /etc/resolv.conf points to nameserver`

`$ useradd hadoop`

`$ su - hadoop`

`$ tar -xzvf hadoop-2.9.1.tar.gz `

`$ sudo su -`

`$ mv hadoop-2.9.1 /opt/.`

`$ cd /opt`

`$ ln -s hadoop-2.7.3 hadoop`

### Setup ".bash_profile"

## Hadoop Configuration files:

  core-site.xml

  hdfs-site.xml

  mapred-site.xml

  yarn-site.xml

## Commands to start services:

`$ hadoop namenode -format`

`$ hadoop-daemon.sh start namenode`

`$ yarn-daemon.sh start resourcemanager`

`$ yarn-daemon.sh start nodemanager`
