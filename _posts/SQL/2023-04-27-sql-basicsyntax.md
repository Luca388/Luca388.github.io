---
layout: post
categories: SQL
tags: sql
title: SQL 기본 문법
---
# DDL (Data Definition Language)
## CREATE
데이터베이스를 생성하거나 테이블을 만들수 있는 DML이다.               
example of creating DataBase:
```sql
CREATE DATABASE my_db;
```
example of creating table
```sql
CREATE TABLE table_name
(
column_name1 data_type(size) [constraint_name],
column_name2 data_type(size) [constraint_name],
column_name3 data_type(size) [constraint_name],
....
);
```
제약조건 생략 가능 생략하면 기본 NULL값.

## Alter
```sql
ALTER TABLE NAME_OF_TABLE 
```
## RENAME

## Drop
```sql
DROP TABLE TABLE_NAME;
# DML(Data Manipulation Languague)
## Select
```sql
select * from dual;
```
## Insert
```sql
INSERT INTO TABLE_NAME(column_list) VALUES (Value_List);
```

## Update
```sql
UPDATE TABLE_NAME SET WANT_TO_CHANGE_COLUMN = NEW_VALUE; 
```
## Delete
```sql 
DELETE FROM NAME_OF_TABLE WHERE conditional_clause;
```
# DCL(Data Control Language)

# TCL(Transaction Control Language)
