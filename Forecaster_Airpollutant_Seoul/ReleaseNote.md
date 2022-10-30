### **Release Note**
#### **2022.10.29**
**Update** 
- 데이터 전처리 수정
	- 기존: 결측치 존재하는 time stamp 의 데이터 drop out
	- 변경: 결측치 & IQR 기준으로 한 이상치에 대하여 linear interpolation
- Hyper parameter
	- 직전 30일 학습 & 다음 stamp 예측
	- hidden size : 18
	- learning rate : 0.002
	- epoch : 600 (early stopping 적용)

**Future work**
dev. ARIMA-LSTM hybrid model
<br>

#### **2022.10.27**
**Update**
- PyTorch의 LSTM 모델을 이용하여 서울특별시 중구의 2017 ~ 2019년 까지의 대기오염물질 중 오존농도 예측.

**to fix**
- coefficient correlation NAN으로 나옴 <- ..?
- 데이터 전처리 중 결측치 처리 과정에서 결측치가 있다면 해당 timestamp 데이터 아묻따 제거해버려서 예측결과에 약간 time shift oo,,
	-> 다른 방법 강구 필요,,
