## First Ubuntu setup and configure

## Install Apt `serviceName`
```sh
sudo apt install
```
## Status Check `serviceName`
```sh
sudo systemctl status 
```

---
### Install Node
```sh
sudo apt install nodejs
```
### Install Npm
```sh
sudo apt install npm -y
```
### Install php
```sh
sudo apt install php
```
### Install Composer
```sh
sudo apt install composer
```
## Laravel Install But laravel Command not found
```sh
export PATH="$HOME/.config/composer/vendor/bin:$PATH"
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
### If you not Set Password, then Username & password
```sh
sudo cat /etc/mysql/debian.cnf
```

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
Next
```sh
sudo mysql_secure_installation
```

Login `http://localhost/phpmyadmin/` UserName `phpmyadmin` Password `---`
 
