# Download jdk8 from browser
https://mega.nz/#!bnBGRILS!pQV6DgaBupwMBFEZdFLSiJAChjkdY4FtgEliwCMOjqw

# through gitbah sending file local to remote
 scp jdk-8u211-linux-x64.rpm root@10.0.11.11:/opt


AFTER COPY THE THE FILE REMOVE OLD JAVA OR JDK USING BELOW COMMANDS
```
yum remove java
yum autoremove java
yum remove jdk
rpm -e java
rpm -e jdk
rpm -qa | grep java
rpm -e package
rpm -e $(rpm -qa | grep java)
```

## install java using below command
rpm -ivh jdk-8u211-linux-x64.rpm

### mobaxterm output

[root@jenkins opt]# update-alternatives --config java

There is 1 program that provides 'java'.

  Selection    Command
-----------------------------------------------
*+ 1           /usr/java/jdk1.8.0_211-amd64/jre/bin/java

Enter to keep the current selection[+], or type selection number: 1


[root@jenkins opt]# cd /usr/
[root@jenkins usr]# ls
bin  etc  games  include  java  lib  lib64  libexec  local  sbin  share  src  tmp
[root@jenkins usr]# cd java
[root@jenkins java]# ls
default  jdk1.8.0_211-amd64  latest
[root@jenkins java]# cd jdk1.8.0_211-amd64/
[root@jenkins jdk1.8.0_211-amd64]# ls
bin        include         jre  LICENSE  README.html  src.zip                             THIRDPARTYLICENSEREADME.txt
COPYRIGHT  javafx-src.zip  lib  man      release      THIRDPARTYLICENSEREADME-JAVAFX.txt
[root@jenkins jdk1.8.0_211-amd64]# export JAVA_HOME=/usr/java/jdk1.8.0_211-amd64
[root@jenkins jdk1.8.0_211-amd64]# echo $JAVA_HOME
/usr/java/jdk1.8.0_211-amd64
[root@jenkins jdk1.8.0_211-amd64]# vi .bash_profile
[root@jenkins jdk1.8.0_211-amd64]# which java
/bin/java
[root@jenkins jdk1.8.0_211-amd64]# java -version
java version "1.8.0_211"
Java(TM) SE Runtime Environment (build 1.8.0_211-b12)
Java HotSpot(TM) 64-Bit Server VM (build 25.211-b12, mixed mode)
[root@jenkins jdk1.8.0_211-amd64]# echo $JAVA_HOME
/usr/java/jdk1.8.0_211-amd64
[root@jenkins jdk1.8.0_211-amd64]# source .bash_profile
[root@jenkins jdk1.8.0_211-amd64]# echo $JAVA_HOME
/usr/java/jdk1.8.0_201-amd64
[root@jenkins jdk1.8.0_211-amd64]# which java
/bin/java
