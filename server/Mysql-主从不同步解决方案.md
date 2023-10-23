mysql>reset slave;
mysql>change master to master_host='10.0.0.170',master_user='sync',master_password='qwertysync',master_log_file='mysql-bin.000007',master_log_pos=154;
mysql>start slave;
