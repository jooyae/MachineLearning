
## SWU MACHINE LEARNING

![image](https://user-images.githubusercontent.com/58849278/117250140-bb36ae00-ae7d-11eb-9586-cce643406bbd.png)

## 머신러닝 알고리즘 종류

 - classification
 - estimation
 - prediction
 - affinity grouping
 - association rules
 - clustering
 - description
 - profiling


## 독립변수 X와 종속변수 Y 형태에 따른 머신러닝 기법 

![image](https://user-images.githubusercontent.com/58849278/117250551-5def2c80-ae7e-11eb-9559-9f327dcdc7d9.png)

## Decision Tree

**Feature 선별할 때 사용하는 규칙 기반의 데이터 분류와 예측** 

![image](https://user-images.githubusercontent.com/58849278/117250709-95f66f80-ae7e-11eb-8021-a445ef443e4a.png)

## 회귀모형

 - 회귀모형의 에러 제곱합 평가 (sum of squares)
	 **SST = SSR + SSE** 
	 - SST = the total sum of squares 
	 - SSR = the regression sum of squares 
	 - SSE = the sum of squares of errors 
	 
 - 회귀모형의 적합도 평가 (R-squared)
		 - R-squared = Explained variance / Total variance 
		 - 변수의 개수가 추가되면 R^2 값은 높아짐
		 - 변수의 개수를 패널티로 보정된 R^2 사용 

![image](https://user-images.githubusercontent.com/58849278/117251497-b7a42680-ae7f-11eb-88ff-bf730327730f.png)		
	

## LinearRegression

1. 50명의 사람의 신체 데이터가 들어있는 csv 파일 준비 

2. head() 메소드 사용하여 randomized people data 출력 

3. matplotlib() 활용하여 데이터 시각화 

4. scikit learn , 선형회귀의 사용으로 예측된 사람의 신체 데이터와 각각의 절편과 기울기 출력

5. 마찬가지로 matplotlib() 사용하여 결과 시각화 

7. Logistic Regression 으로 예측률 보완 

	![image](https://user-images.githubusercontent.com/58849278/117252311-bde6d280-ae80-11eb-8e09-58fd95b6b8f5.png)

## Logistic Regression

1. 비행기 탑승 승객 리스트 ID, Survival, Class, Gender, Age 순으로 수치화한 데이터 (.csv) 불러오기 

2. 생존을 예측하는 분류기 생성 (예측 변수 2개) 

3. 추정 확률과 결정 경계를 시각화하여 출력 

![image](https://user-images.githubusercontent.com/58849278/117253118-d1466d80-ae81-11eb-8757-1a0c970c85c4.png)


 ## Ensemble Learning

앙상블 학습은 여러 모델이 동일한 문제를 해결하고 더 나은 결과를 얻도록 훈련시키는 기계 학습 모델이다. 
주된 가설은 약한 모델이 올바르게 결합되면 더 정확하고 견고한 모델을 얻을 수 있다는 것이다. 
낮은 편향과 낮은 분산은 반대 방향으로 가장 많이 변하지만 편향과 분산은 작업중인 데이터의 근본적인 복잡성을 해결하기에 중요한 기능을 한다. 자유도가 너무 크지 않은 모델을 만들기 위해 우리는 앙상블 학습을 사용하며 배깅, 부스팅, 스태킹 알고리즘을 상황에 맞게 활용해야 한다. 

 - bagging & pasting
 무작위로 훈련 데이터 셋을 잘게 나눈 뒤 나누어진 훈련 데이터 셋을 여러 개의 모델에 할당하여 학습시키는 방식 
 (1) Bagging : 중복 허용, 리샘플링 , 복원 추출
 (2) Pasting : 중복 허용하지 않고 훈련 데이터 셋 나눔
 ![image](https://user-images.githubusercontent.com/58849278/117254127-fbe4f600-ae82-11eb-9326-be71db03ba81.png)
 - ada boosting & gradient boosting
 
	(1) 에이다 부스트
	Weak Model 을 순차적으로 적용해나가는 과정에서 잘 분류된 샘플의 가중치는 낮추고 잘못 분류된 가중치를 상대적으로 점점 높여 주면서 샘플 분포를 변화시키는 원리 

	(2) 그레디언트 부스트 
Weak Model 을 순차적으로 적용해나가는 과정에서 잘못 분류된 샘플의 error를 optimization하는 원리 
식별하기 쉬운 데이터 특징에 대응하는 학습기부터 식별하기 어려운 데이터 특징에 대응하는 학습기까지 자동 생성됨 

	 ![image](https://user-images.githubusercontent.com/58849278/117254232-20d96900-ae83-11eb-92f9-419e927ace9f.png)

 



