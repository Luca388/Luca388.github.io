---
layout: post
categories: assembly
tags: x86
title: assembly data type
---
크기 지정자는 메모리 피연산자 ( [] ) 앞에 TYPE PTR 형태로 추가될수 있으며  타입은 다음과 같다
- BYTE PTR
> 1 byte의 크기를 지정한다
- WORD PTR 
> 2byte의 크기를 지정한다
- DWORD PTR 
> 4byte 의 크기를 지정한다
- QWORD PTR
> 8byte 의 크기를 지정한다


각각의 TYPE PTR을 사용해 TYPE 만큼 값을 참조할수 있다  
예시    

|피연산자|설명|
|-|-|
|QWORD PTR[0x8048000]|0x8048000의 데이터를 8바이트만큼 참조|
|DWORD PTR[0x8048000]|0x8048000의 데이터를 4바이트만큼 참조|
|WORD PTR[rax]|rax가 가르키는 주소에서 데이터를 2바이트만큼 참조|



# reference 
dreamhack
