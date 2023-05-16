---
layout: post
categories: SQL
tags: oracle
title: ROLLUP 과 CUBE 의 차이
---
# ROLLUP
!()[https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Fp9c2J%2Fbtrb1c2Ueeu%2FzcK1NtXCOGskC4ha6N5Jek%2Fimg.png]

소그룹 간의 합계를 계산하는 함수이다.
ROLLUP을 이용하면 GROUP BY 로 묶은 각각의 소그룹 합계와 전체 합계를 모두 구할수 있다.
```sql
SELECT 상품ID, 월, SUM(매출액) AS 매출액
FROM 월별매출
GROUP BY ROLLUP(상품ID, 월);
```

> 맨 처음 명시한 컬럼에 대해서만 소그룹 합계를 구해준다.

# CUBE
!()[https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FbnZqja%2FbtrbV1uygXO%2FsDSQBLXRbfaCniIcTgQZgk%2Fimg.png]       

CUBE함수는 항목들 간의 다차원적인 소계를 계산한다. ROLLUP과 달리 GROUP BY절에 명시한 모든 컬럼에 대해 소그룹 합계를 계산한다.


# reference
<https://for-my-wealthy-life.tistory.com/44>