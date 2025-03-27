## First Ubuntu setup and configure

## Install Apt `serviceName`
```sh
sudo apt install
```
## Status Check `serviceName`
```sh
sudo systemctl status 
```

### Install Node
```sh
sudo apt install nodejs
```
### Install php
```sh
sudo apt install php
```
### Install Composer
```sh
sudo apt install composer
```
---
## Configure Server 

### Install Apache 
```sh
sudo apt install apache2
```
### Install Mysql
```sh
sudo apt install mysql-server
```

### Install Phpmyadmin
```sh
sudo apt install phpmyadmin
```

### Configure Phpmyadmin
```sh
sudo ln -s /usr/share/phpmyadmin /var/www/html/phpmyadmin
```
---
### If Change Password Phpmyadmin
```sh
 sudo mysql -u root -p
```
Then
```sh
ALTER USER 'phpmyadmin'@'localhost' IDENTIFIED BY '---';
FLUSH PRIVILEGES;
EXIT;
```

Login `http://localhost/phpmyadmin/` UserName `phpmyadmin` Password `---`
