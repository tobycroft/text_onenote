关闭selinux
setenforce 0; 

vi /etc/sysconfig/selinux
SELINUX=enforcing 改为 SELINUX=disabled
