# MySQL

## Start mysql

```bash
sudo service mysql restart
```

## Entering and exiting mysql shell

```bash
sudo mysql
```

```sql
EXIT;
```

## Creating admin user

```sql
CREATE USER 'dbadmin'@'%' IDENTIFIED BY 'password_here';

GRANT ALL PRIVILEGES ON *.* TO 'dbadmin'@'%';

FLUSH PRIVILEGES;
```

## Change user password

```sql
ALTER USER 'root'@'%' IDENTIFIED BY 'new_password_here';
```

## Grant all permissions

```sql
GRANT ALL PRIVILEGES ON *.* TO 'dbadmin'@'%';

FLUSH PRIVILEGES;
```

## Create database

```sql
CREATE DATABASE new_database;
```
