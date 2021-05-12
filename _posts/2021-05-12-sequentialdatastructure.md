---
title: "순차적 자료구조"
author: Young Dean
date: 2021-05-12
categories: [CS]
tags: [CS, datastructure]
toc: true
toc_sticky: true
---

> 해당 게시물은 신찬수 교수님의 자료구조 강의를 듣고 이해한 내용을 바탕으로 작성하였습니다. 
> [링크](https://www.youtube.com/watch?v=buJBlTsWlW0&list=PLsMufJgu5933ZkBCHS7bQTx0bncjwi4PK&index=7)

# 순차적 자료구조(Sequential data structure) 소개

1. ```배열```, ```리스트```
2. 배열과 리스트와 비교하여 제한된 접근으로 허용되는 자료구조 : ```Stack```, ```Queue```, ```dequeue```
3. ```Linked list(연결리스트)```

아래의 각 자료구조는 공부 후 포스팅하고 링크를 추가할 예정

## Stack
- ```LIFO(Last In First Out)```
- 맨 아래부터 쌓아가고 나올 때는 맨 위의 값이 나오게 됨.

## Queue
- ```FIFO(First In First Out)```
- 선착순 

## dequeue
- ```Stack```과 ```Queue```를 합쳐놓은 것

## Linked list(연결리스트)
- 띄엄띄엄 값이 저장되어있으면 다음 값이 어디 저장 되어있는지 알고 연결한 구조
- 마지막은 C언어에서 ```NULL```, Python에서는 ```None```을 가리킴, 즉 아무것도 없음을 나타냄
- 인덱스로 접근할 수 없음
