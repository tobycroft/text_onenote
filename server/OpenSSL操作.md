linux下
步骤1：生成密钥
命令：openssl genrsa 1024 > server.key
说明：这是用128位rsa算法生成密钥，得到server.key文件
步骤2: 生成证书请求文件
命令：openssl req -new -key server.key > server.csr
说明：这是用步骤1的密钥生成证书请求文件server.csr, 这一步提很多问题，一一输入
步骤3: 生成证书
命令：openssl req -x509 -days 365 -key server.key -in server.csr > server.crt
说明：这是用步骤1,2的的密钥和证书请求生成证书server.crt，-days参数指明证书有效期，单位为天
window下
步骤1：生成密钥
命令：openssl genrsa 1024 > server.key
说明：这是用128位rsa算法生成密钥，得到server.key文件
步骤2: 生成证书请求文件
命令：openssl req -config D:\phpStudy\Apache\conf\openssl.cnf -new -key server.key > server.csr
说明：这是用步骤1的密钥生成证书请求文件server.csr, 这一步提很多问题，一一输入
步骤3: 生成证书
命令：openssl req -config D:\work_soft\Apache2.2\conf\openssl.cnf -x509 -days 365 -key server.key -in server.csr > server.crt
说明：这是用步骤1,2的的密钥和证书请求生成证书server.crt，-days参数指明证书有效期，单位为天
把得到的server.key和server.crt文件拷贝到apache的对应目录
