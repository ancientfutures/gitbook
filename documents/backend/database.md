---
description: MariaDB
---

# Database

Basic command **mysql:**

```
$ mysql -u root -p —— login mysql
$ CREATE DATABASE 'yourDB';
$ SHOW DATABASES;
$ CREATE USER 'user1'@localhost IDENTIFIED BY 'password1';
$ SELECT User FROM mysql.user;
$ GRANT ALL PRIVILEGES ON *.* TO 'user1'@localhost IDENTIFIED BY 'password1';

To grant privileges only for yourDB, type the following statement:
$ GRANT ALL PRIVILEGES ON 'yourDB'.* TO 'user1'@localhost; 
$ FLUSH PRIVILEGES;
$ SHOW GRANTS FOR 'user1'@localhost;

$ use 'database';
& show tables;
```

Export & Import

```
$ mysqldump -u root -p database > file.sql —— export
$ mysqldump -u root -p database < file.sql —— import
```
