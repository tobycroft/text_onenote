sudo yum install nfs-utils -y
mkdir /upload
echo "78ae3485d0-gmy8.ap-southeast-1.nas.aliyuncs.com:/ /upload  nfs4 vers=4.0,rsize=1048576,wsize=1048576,hard,timeo=600,retrans=2,_netdev,noresvport 0 0">>/etc/fstab

mount -t nfs -o vers=4.0,noresvport 78ae3485d0-gmy8.ap-southeast-1.nas.aliyuncs.com:/ /upload
ln -s /upload /www/wwwroot/MChat/public/

ln -s /upload /www/wwwroot/MChat_adm/public/
