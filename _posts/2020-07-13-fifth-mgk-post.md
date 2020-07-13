---
title: "2020년 7월 13일 모각코 4일차"
date: 2020-07-13
categories: 
 - MGK
 - 모각코
--- 

### 2020년 7월 13일 모각코 4일차 진행  
+ 금일의 모각코 진행 목표  
 1.이분탐색, 해쉬, 이진 검색 트리, 힙 알고리즘 공부하고 알고리즘 문제 1개 풀기  
 2. React & Redux: 리덕스로 앱 스테이트 관리하기
 
   
+ 금일의 모각코 진행 결과  
 1. 이분탐색, 해쉬, 이진 검색 트리, 힙 알고리즘에 대해 이미 이론은 알고 있어서 빠르게 복습하고 프로그래머스에서 해시에 해당하는 ["완주하지 못한 선수"](https://programmers.co.kr/learn/courses/30/lessons/42576?language=python3)문제를 풀었다.  
 ```python  
 def solution(participant, completion):  
     runners = {}  
     for i in range(len(participant)):  
         if participant[i] in runners:  
             runners[participant[i]] += 1  
         else:  
             runners[participant[i]] = 1  
     for i in range(len(completion)):  
         if completion[i] in runners:  
             runners[completion[i]] -= 1  
     answer = ''  
     for i in range(len(participant)):   
         if participant[i] in runners:  
             if runners[participant[i]] != 0:  
                 answer = participant[i]  
                 break  
     return answer  
 ```    
해시와 같이 구현하기 위하여 key-value 쌍을 갖는 파이썬의 딕셔너리를 이용하여 문제를 해결하였다.  
일단 participant에 해당하는 값들을 key로 하고 이들의 value는 기본적으로 1로 설정하되, 동명이인이 있는 경우 value값을 1만큼 증가시켰다.  
이후 completion에 해당하는 값들을 딕셔너리의 key에서 찾아 value값을 1 씩 감소시켰다.  
최종적으로 딕셔너리에서 value값이 0이 아닌 경우, 완주하지 못한 사람이므로 이를 리턴하였다.  
프로그래머스에서 푸는 알고리즘은 처음이었는데 문제 난이도는 쉬웠던것 같다. 
   
 2. React & Redux: 리덕스로 앱 스테이트 관리하기  
 라덕스의컨테이너, 리듀서, 액션을 사용하여 책 정보를 알수 있는 페이지를 제작하였다.  
 <img src="https://user-images.githubusercontent.com/28749734/87317434-f1f3ae80-c561-11ea-97dd-b0c599dfddde.png" width="50%" height="300">
 <img src="https://user-images.githubusercontent.com/28749734/87317453-fcae4380-c561-11ea-9284-6d1f9965e617.png" width="50%" height="300">  
 아직 리액트에 익숙하지 않은데 리덕스를 공부하려고 하니 너무 어렵게 느껴진다. 조금 쉬운 강의를 알아봐서 변경하던지 해야겠다.  
 
 
