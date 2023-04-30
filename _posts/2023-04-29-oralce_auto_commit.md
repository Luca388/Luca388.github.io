---
layout: post
title: Oracle and SQL Server Auto Comiit
categories: SQL
tags: oracle
---
# ORACLE
DDL
> - unable Rollback
- Auto Commit
- DDL문장의 수행은 내부적으로 트랜젝션을 종료 시킨다.

DML
> - Can Rollback before Commit
- User commit

# 논리연산자 우선순위
NOT > AND > OR


# NULL 과의 연산

NULL + 1 == NULL

#  비교연산
FALSE 리턴
 
# 부정 비교연산
iso 표준

- != : 같지않다
- ^- : 같지않다
- <> : 같지않다

# tip
oracle 에서 insert into vaule 에 ''가 삽입되면 NULL값으로 처리된다

# SQL Server
DDL
> DDL 문장 수행후 자동으로 commit을 수행하지 않는다.

# tip
SQL Server 에서  insert into 값에 ''가 들어가면 ''로 조회가 가능하다
