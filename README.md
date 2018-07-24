# Hadoop-QuickStart

Maven libraries from Hadoop

## Hadoop denpendecies:

$ `sudo su -`

$ `yum update -y`

$ `yum install wget -y`

$ `yum install nano -y`

$ `wget --no-cookies --no-check-certificate --header "Cookie: gpw_e24=http%3A%2F%2Fwww.oracle.com%2F; oraclelicense=accept-securebackup-cookie" "http://download.oracle.com/otn-pub/java/jdk/8u181-b13/96a7b8442fe848ef90c96a2fad6ed6d1/jdk-8u181-linux-x64.rpm"
`

$ `rpm -Uvh jdk-8u181-linux-x64.rpm`

$ ` alternatives --config java`

$ ` alternatives --config javac`

$ ` sh -c "echo export JAVA_HOME=/usr/java/latest/jre >> /etc/environment"`

$ ` source /etc/environment`

$ ` echo $JAVA_HOME`

## Install Hadoop instructions:

$ `sudo su -`

$ `chkconfig iptables off; service iptables stop`

$ `nano /etc/resolv.conf points to nameserver`

$ `useradd hadoop`

$ `su - hadoop`

$ `ssh-keygen -t rsa -P ""`

$ `exit`

$ `chmod -R 650 /home/hadoop/.ssh`

$ `nano /etc/ssh/sshd_config` change PasswordAuthentication ( no ) to yes

$ `systemctl restart sshd`

$ `ssh-copy-id -i .ssh/id_rsa.pub localhost`

$ `ssh localhost`

$ `exit`

$ `tar -xzvf hadoop-2.9.1.tar.gz `

$ `sudo su -`

$ `mv hadoop-2.9.1 /opt/.`

$ `cd /opt`

$ `ln -s hadoop-2.7.3 hadoop`

## Hadoop Configuration files:

  Setup ".bash_profile"

  core-site.xml

  hdfs-site.xml

  mapred-site.xml

  yarn-site.xml

## Commands to start services:

$ `hadoop namenode -format`

$ `hadoop-daemon.sh start namenode`

$ `hadoop-daemon.sh start datanode`

$ `yarn-daemon.sh start resourcemanager`

$ `yarn-daemon.sh start nodemanager`
