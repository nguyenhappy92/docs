10.11.23.140 master01
10.50.50.141 master01

# I. Both Master Server

yum install epel-release -y
yum update -y
vi /etc/yum.repos.d/mariadb.repo
```# MariaDB 10.2 CentOS repository list - created 2019-09-20 16:34 UTC
# http://downloads.mariadb.org/mariadb/repositories/
[mariadb]
name = MariaDB
baseurl = http://yum.mariadb.org/10.2/centos7-amd64
gpgkey=https://yum.mariadb.org/RPM-GPG-KEY-MariaDB
gpgcheck=1```
=> Create repo at link https://downloads.mariadb.org/mariadb/repositories
yum install MariaDB-server MariaDB-client -y
/usr/bin/mysql_secure_installation
vi /root/.my.cnf
[client]
  user            =root
  password        =ye74b87EYP7CsdAFDD
chmod 400 /root/.my.cnf
