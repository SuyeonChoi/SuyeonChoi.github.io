---
title: "[Python/DL]TIL-5th week"
date: 2020-09-08
categories: 
 - TIL
---  

## 20200908
### 파이썬 웹 개발(진도율 10%)  
 - 08.Flask 기초: 01.03.MVC란   

## 20200909
### 파이썬 웹 개발(진도율 12%)  
 - 02.웹 기본 및 프론트엔드 기초: 21.04. ~ 29.04. HTML, CSS(2)    
 - [Django 공식 웹사이트 메인 페이지 제작](https://github.com/SuyeonChoi/TIL/tree/master/Python%20Web%20Developement/02.%20%EC%9B%B9%20%EA%B8%B0%EB%B3%B8%20%EB%B0%8F%20%ED%94%84%EB%A1%A0%ED%8A%B8%EC%97%94%EB%93%9C%20%EA%B8%B0%EC%B4%88/HTML%2CCSS(2))   
 <img width="80%" alt="캡처" src="https://user-images.githubusercontent.com/28749734/92678089-27e5c100-f360-11ea-8d2f-4620a901be47.PNG">  

## 20200910
### 파이썬 웹 개발(진도율 13%)
 - 02.웹 기본 및 프론트엔드 기초: 30.05. ~ 33.05. Git, Github  
 
## 20200911
### 딥러닝/인공지능(진도율 8%)
 - PART1.인공지능에 대한 개념과 준비: 01.~03. 인공지능 개념 이해  
 - 딥러닝의 학습 과정  
 <img width="560" alt="ai_1" src="https://user-images.githubusercontent.com/28749734/92939928-62974880-f489-11ea-8f98-cb294bd96bcd.PNG">  
 - 딥러닝 용어  
   + Convolution : 합성법. 합성을 하여 이미지의 특징을 추출하는 것  
   + Pooling Layer: 이미지가 가진 특징으로 압축  
   + Optimization: 최적화  
   + Activation Function: 함수에 따라 불필요한 값 제거  
   + Softmax: 값들을 확률로 변형  
      
## 20200913  
### 딥러닝/인공지능(진도율 8%)  
 - PART1.인공지능에 대한 개념과 준비: 04.~05. 인공지능 개념 이해  
 - 딥러닝 용어  
   + Learning Rate: 하이퍼 파라미터. 학습시 사람이 cost를 직접 적절하게 조절하는 것   
   + Batch Size: 모든 데이터를 한번에 모델에 넣어줄 수 없으므로 얼마나 나누어(batch)로 조절하는 크기   
   + Epoch / Step: 인공지능이 반복하는 수  
   + Train / Validation / Test: 크게 train과 test로 나눔. train-훈련, test-테스트  
   <img width="391" alt="train" src="https://user-images.githubusercontent.com/28749734/92999529-79f33600-f55c-11ea-8022-eb4a1c81c0d6.PNG">  
   + Label / Ground Truth: 모델 데이터셋에 대한 정답  
 - CNN 모델 구조   
   + Feature Extraction / Classification: Convolution 필터로 특징 추출
   + Convolution Layer: 필터(패턴)에 따라 특징 합성.추출  
   + Pooling Layer(Max Pooling): 값이 높은 것(중요한 것)을 추출 ex) 이미지 압축  
   + Activation Function(ReLU): 불필요한 것 제거  
   + Fully Connect: 계산하여 예측  
   + 보통 Convolution ~ Activation을 반복한 것으로 Fully Connect를 하는 과정으로 이루어짐  