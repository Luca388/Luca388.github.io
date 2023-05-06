---
layout: post
categories: SQL
tags: MSSQL
title:  top 함수와 top with ties 함수[MSSQL]
---
# TOP WITH TIES
TOP 과 동일하게 상위 N개의 데이터를 조회한다.

하지만 동일한 데이터가 있을 경우 함께 출력된다. 

 

TOP WITH TIES를 사용하기 위해서는 ORDER BY 절이 반드시 함께 와야 한다. (TOP의 경우 없어도 가능)

동일한 데이터는 ORDER BY절 뒤의 오는 컬럼이 기준이 된다.

