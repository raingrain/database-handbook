# 基本语法

## DDL

***Data Definition Language，数据定义语言，用来定义数据库、表、字段。***

---

### 查询所有数据库

> - ***show databases;***

---

### 查询当前数据库

> - ***select database();***

---

### 创建数据库

> - ***create database [if not exists] 数据库名 [default charset 字符集] [collate 排序规则];***

---

### 删除数据库

> - ***drop database [if exists] 数据库名;***

---

### 使用数据库

> - ***use 数据库名;***
> - **tips:**
>   - `sys` 是系统数据库。

---

### 查询当前数据库所有表

> - ***show tables;***

---

### 查询表结构

> - ***desc 表名;***

---

### 查询指定表的建表语句

> - ***show create table 表名;***

---

### 创建表

> - ***create table 表名(字段1 字段1类型 [comment 字段1注释], 字段2 字段2类型 [comment 字段2注释], ..., 字段n 字段n类型 [comment 字段n注释]) [comment 表注释];***

---

### 添加字段

> - ***alter table 表名 add 字段名 数据类型(长度) [comment 注释] [约束];***

---

### 修改字段的数据类型

> - ***alter table 表名 modify 字段名 新数据类型(长度);***

---

### 修改字段的名字和数据类型

> - ***alter table 表名 change 旧字段名 新字段名 新数据类型(长度) [comment 注释] [约束];***

---

### 删除字段

> - ***alter table 表名 drop 字段名;***

---

### 修改表名

> - ***alter table 表名 rename to 新表名;***

---

### 删除表

> - ***drop table [if exists] 表名;***

---

### 删除表并重新创建该表

> - ***truncate table 表名;***

---

## DML

***Data Manipulation Language，数据操作语言，用来对数据库表中的数据进行增加、删除和修改。***

## DQL

***Data Query Language，数据查询语言，用来查询数据库表中的记录。***

## DCL

***Data Control Language，数据控制语言，用来创建数据库用户以及控制数据库的访问权限。***
