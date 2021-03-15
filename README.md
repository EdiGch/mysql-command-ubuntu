# Mysql command

## Install mysql:

```sudo apt update```

```sudo apt install mysql-server```

```mysql --version```

```sudo mysql_secure_installation```
Y 0 New password 'newPassword20'

### Trubel shutting

Ennror access denied for user

```sudo mysql```

```show databases;```

```use mysql```

```select user,host,plugin from mysql.user;```

### Create a new user and assign him permissions

```create user 'userName'@'localhost' identified by 'newPassword20';```

```grant all privileges on *.* to 'userName'@'localhost';```

```update user set plugin="auth_socket" where User='userName';```

```CREATE USER 'admin'@'localhost' IDENTIFIED BY 'admin';```

```GRANT ALL PRIVILEGES ON *.* TO 'admin'@'localhost' WITH GRANT OPTION;```

```flush privileges;```

```exit;```

```sudo service mysql restart```

```mysql -u gcharkiewicz -p```

### Create database:

```sudo mysql```

```mysql -u root -p```

```CREATE DATABASE bundleShop_db;```


Delete all mysql
https://linuxscriptshub.com/uninstall-completely-remove-mysql-ubuntu-16-04/
