---
title: "2020년 7월 27일 모각코 6일차"
date: 2020-07-27
categories: 
 - MGK  
 - 모각코
---  
 
### 2020년 7월 27일 모각코 6일차 진행  
+ 금일의 모각코 진행 목표  
 1. 자료구조 복습 - ArrayList 
 2. 졸업 프로젝트 데이터베이스 - 스키마 생성 
 3. 알고리즘 문제 1개 풀기  
   
+ 금일의 모각코 진행 결과  
 1. 자료구조 복습_JAVA  
   - 자바의 ArrayList 내장 함수를 이용하여 Stack과 Queue 인터페이스를 구현하였다.  
   - remove 함수를 하게 되면 해당 인덱스가 비어있는 것이 아니라 그만큼 배열이 가득 차도록 재배열 된다는 것을 알게되었다.  
   - [Repository](https://github.com/SuyeonChoi/Assignments/tree/master/DataStructure%20Review/java.util.ArrayList)에 push 하였다.  
 2. [BOJ 문제](https://github.com/cnu-pai/2020SUMMER-AlgorithmStudy/blob/master/%EC%B5%9C%EC%88%98%EC%97%B0/p18808.py)_Python   
   - Gold 3 수준의 문제를 풀고 [깃레퍼짓토리](https://github.com/cnu-pai/2020SUMMER-AlgorithmStudy/blob/master/%EC%B5%9C%EC%88%98%EC%97%B0/p18808.py)d에 push하였다.  
   - 알고리즘 풀이 설명:  
   ```python  
   N, M, K = map(int, input().split())  
   note = [[0]*M for _ in range(N)]  
   
   def isFitted(r, c, x, y, sticker):  
       for i in range(r):  
           for j in range(c):  
               if sticker[i][j] == 1 and note[x+i][y+j] == 1:  
                   return False  
       for i in range(r):  
           for j in range(c):  
               if sticker[i][j] == 1 and note[x+i][y+j] == 0:  
                   note[x+i][y+j] = 1  
       return True  
   
   
   def rotate(r, c, sticker):  
       transform = [[0]*r for _ in range(c)]  
       p = r  
       for i in range(r):  
           p -= 1  
           for j in range(c):  
               transform[j][p] = sticker[i][j]  
       return transform, c, r  
   
   
   for s in range(K):  
       R, C = map(int, input().split())  
       sticker = [list(map(int, input().split())) for _ in range(R)]  
       isfit = False  
       for r in range(4):  
           for i in range(N):  
               if N - i < R:  
                   continue  
               for j in range(M):  
                   if M - j < C:  
                       break  
                   if isFitted(R, C, i, j, sticker):  
                       isfit = True  
                       break  
               if isfit == True:  
                   break  
           if isfit == True:  
               break  
           sticker, R, C = rotate(R, C, sticker)  
   
   
     
   result = 0  
   for i in range(N):  
       for j in range(M):  
           if note[i][j] == 1:  
               result += 1  
   print(result)  
        
   ```   
   모든 경우의 수에 대한 계산을 하는 방식으로  
   (1) 왼쪽 가장 위쪽부터 시작하여 스티커를 붙일 수 있는지  
   (2) 없다면, 90도, 180도, 270도로 회전한 경우 가능한지  
   에 대한 경우를 모두 계산하는 방식으로 구현하였다.  
   나는 (1)을 구현하는 것이 처음에는 생각하기 까다롭다고 그냥 한번 체크한 뒤 되는 경우 마킹을 하면서 체크하는 간단한 방법이 시간 제한에 제한받지 않아 쉽게 구현할 수 있었다.  
     
 3. 졸업프로젝트 데이터베이스  
   - 알고리즘을 풀고 나니 시간이 부족하여 도움될만한 영상을 시청: [Build a GraphQL Server with Node.js and Redis](https://www.youtube.com/watch?v=_Zwqn7FV6ms)   
 
