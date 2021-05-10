---
title: "Python List vs Dict vs Tuple"
author: Young Dean
date: 2021-05-10
categories: [Lang_Python]
tags: [Python]
toc: true
toc_sticky: true
---
# Python ```[]```, ```{}```, ```()```의 차이

## list ```[]```
```[]```는 파이썬의 리스트 자료형에서 사용한다. 
```Python
member_name = [] # 요런 식으로 빈 배열을 선언가능
member_id = [1012, 1013, 1014] # 원소를 넣어 선언 간능
print(member_id[2]) # 0번부터 시작해서 2인덱스에 해당하는 원소를 출력
```

## Dictionary ```{}```
```{}```는 파이썬의 dictionary에서 사용한다. 
list와 닮은 듯 하지만 차이점은 key값과 value를 대응시킨다고 생각하면 된다.

list의 인덱스에는 str형이 들어갈 수 없지만 dict의 key값에는 str형을 넣을 수 있다. 

최근 코딩테스트 문제를 풀다가 처음 사용해보았다.  
[프로그래머스 카카오톡 오픈채팅방 문제 확인하기](https://programmers.co.kr/learn/courses/30/lessons/42888)

```Python
member_name = {} # Dictionary 형식으로 선언
splited_data = i.split() 
# splited_data[1]은 id로 str 형으로 주어짐
# splited_data[2]는 str형의 닉네임을 저장
member_name[splited_data[1]] = splited_data[2] 
```

처음에는 ```member_name```을 ```[]```으로 선언했다가 str형이 들어갈 수 없다고 해서 당황했던 기억이 있다. 

## Tuple ```()```
```()```는 파이썬의 tuple 타입이 사용한다. 
튜플을 선언하고 초기화하는데 ```()```를 사용하고, 원소에 접근할 때는 리스트처럼 ```[]```를 사용한다. 

list와의 차이점은 원소를 제거하거나 변경할 수 없다.

사용 예시는 list와 비슷하며 다음과 같다.

```Python
member_name = () # 요런 식으로 빈 배열을 선언가능
member_id = (1012, 1013, 1014) # 원소를 넣어 선언 간능
print(member_id[2]) # 원소에 접근할 때는 []를 사용
```
