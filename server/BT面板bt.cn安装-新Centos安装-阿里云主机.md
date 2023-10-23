yum install -y screen
screen
mkdir -p /www
mkfs.ext4 /dev/vdb1
mkfs.ext4 /dev/vdb1
echo " /dev/vdb1          /www         ext4           defaults            0 0" >> /etc/fstab
mount -a
yum install -y wget && wget -O install.sh http://download.bt.cn/install/install.sh && sh install.sh
y



wget http://download.yunsuo.com.cn/v3/yunsuo_agent_64bit.tar.gz && tar xvzf yunsuo_agent_64bit.tar.gz && chmod +x yunsuo_install/install && yunsuo_install/install
