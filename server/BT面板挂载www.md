echo " /dev/vdb          /www         xfs           defaults            0 0" >> /etc/fstab
mkdir -p /www
mkfs.xfs /dev/vdb
mount -a

yum install -y wget && wget -O install.sh http://download.bt.cn/install/install.sh && sh install.sh

echo " /dev/vdb          /wallet         xfs           defaults            0 0" >> /etc/fstab
mkdir -p /wallet
mkfs.xfs /dev/vdb
mount -a
