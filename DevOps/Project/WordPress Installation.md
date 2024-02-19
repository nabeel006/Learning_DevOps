### Step 1 
Creating a MySQL Database and User for WordPress
```mysql

sudo mysql
mysql -u root -p

CREATE DATABASE wordpress DEFAULT CHARACTER SET utf8 COLLATE utf8_unicode_ci;
CREATE DATABASE eathcoast_main
SHOW databases;
DROP DATABASE mydatabase;


GRANT ALL ON wordpress.* TO 'admin'@'%';
FLUSH PRIVILEGES;




```

#### How to get database dump
```mysql
source /home/earthcoast_ecdb88to7.sql;

```
#### Change the Database
```mysql

USE earthcoast_main;
Database changed
mysql> SHOW TABLES;
+-------------------------------------------------+
| Tables_in_earthcoast_main                       |
+-------------------------------------------------+
| dof9RHaD_actionscheduler_actions                |
| dof9RHaD_actionscheduler_claims                 |
| dof9RHaD_actionscheduler_groups                 |
| dof9RHaD_actionscheduler_logs                   |


USE earthcoast_proposal;
```
### Step 2
Installing Additional PHP Extentions
sudo apt update