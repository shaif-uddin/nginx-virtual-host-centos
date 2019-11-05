# nginx-virtual-host-centos
Configure virtual in  Nginx in CentOS using Vagrant
OS : CentOS 8

Step1: Create a file /etc/nginx/conf.d/vagrant.local.conf
For WordPress follow this setting in vagrant.local.conf

Step 2: from terminal continue this command.
============================================
mysql -u root -p

CREATE DATABASE wordpress CHARACTER SET utf8mb4 COLLATE utf8mb4_general_ci;
GRANT ALL ON wordpress.* TO 'wordpressuser'@'localhost' IDENTIFIED BY 'change-with-strong-password';
FLUSH PRIVILEGES;
EXIT;


