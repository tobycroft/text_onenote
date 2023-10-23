1） 检查selinux状态
  # getenforce    ##显示为disabled则为成功关闭
2） 关闭selinux。修改/etc/sysconfig/selinux文件，将enforcing改为disabled，重启服务器。
# vim /etc/sysconfig/selinux

安装云锁
注意：如曾经下载过云锁安装包，则将旧的云锁安装包及安装目录删除（rm -rf yunsuo_*）后再安装。
快速安装
wget http://download.yunsuo.com.cn/v3/yunsuo_agent_64bit.tar.gz && tar xvzf yunsuo_agent_64bit.tar.gz && chmod +x yunsuo_install/install && yunsuo_install/install