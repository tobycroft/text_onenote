yum install cifs-utils -y

mount -t cifs -o rw,iocharset=utf8,dir_mode=0777,file_mode=0777,uid=www,gid=www,username=guest,password=guest//7b6ef48c55-emp75.ap-southeast-1.nas.aliyuncs.com  /images
