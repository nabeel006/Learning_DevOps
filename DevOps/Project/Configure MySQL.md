
``` mysql
#shows the password policy
mysql> SHOW VARIABLES LIKE 'validate_password%';

#show all users
mysql> SELECT user, host FROM mysql.user;

#Create User 

CREATE USER 'admin'@'%' IDENTIFIED BY 'admin';

#Grant Permission

GRANT PRIVILEGE ON database.table TO 'admin'@'%';
#If it not work then apply this command

GRANT CREATE, ALTER, DROP, INSERT, UPDATE, INDEX, DELETE, SELECT, REFERENCES, RELOAD on *.* TO 'admin'@'%' WITH GRANT OPTION;
```


*Give All Permission*
```mysql
#Warning: Some users may want to grant their MySQL user the `ALL PRIVILEGES` privilege, which will provide them with broad superuser privileges akin to the **root** user’s privileges, like so:
GRANT ALL PRIVILEGES ON *.* TO 'admin'@'%localhost%' WITH GRANT OPTION;
```

```mysql
#This will free up any memory that the server cached as a result of the preceding `CREATE USER` and `GRANT` statements

FLUSH PRIVILEGES;
exit
```

### Login as New User

```mysql
mysql -u admin -p
```

You can try connecting to the database using the `mysqladmin` tool,
```mysql
sudo mysqladmin -p -u sammy version
```
