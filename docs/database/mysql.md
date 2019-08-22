---
sidebarDepth: 2
meta:
  - name: keywordsv
    content: 数据库 MySQL MySql sql
  - name: description
    content: 本文章主要记录数据库的一些常见网站以及博客。
---


# MySQL 数据库基础操作


数据库版本：`8.0.17`

## 链接语法


```js
// 登录
mysql -u root -p

```

## 密码操作

```js
// 设置密码
set password for root@localhost=password('新密码'); (方法一)
alter user user() identified by '新密码'; (方法二)

// 设置密码时使用加密方式
alter user 'root'@'localhost' identified  with mysql_native_password by  '密码';

// 刷新权限
flush privileges
```


## 数据库操作

### 显示数据库

```js
// 显示数据库
show databases;
```

### 选择数据库

```js
// 选择数据库
use  数据库名;
```

### 查看数据库状态

```js
// 查看数据库状态
status;
```


### 创建数据库

```js
// 创建数据库
create database 数据库名; 

// 创建数据库并设置uff8编码
create database 数据库名 default character set utf8 collate utf8_general_ci; 
```

### 删除数据库

```js
// 删除数据库
drop database 数据库名
```

### 修改数据库

```js
// 修改数据库字符编码
use 数据库名; //进入要修改的数据库
alter database character set utf8;
```


## 数据表操作

### 显示数据表

```js
//显示数据表
show tables;
```

### 创建数据表

```js
//显示数据表
create table people(
  id INT NOT NULL
  name VARCHAR(10)
  age INT
  sex 
)
```


### 显示数据表

```js
//显示数据表
show tables;
```

### 显示数据表

```js
//显示数据表
show tables;
```

### 显示数据表

```js
//显示数据表
show tables;
```

### 显示数据表

```js
//显示数据表
show tables;
```

### 显示数据表

```js
//显示数据表
show tables;
```

### 显示数据表
```js
//显示数据表
show tables;
```



## 备份操作