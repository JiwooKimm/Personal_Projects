### **Release Note**

#### **2022.10.27**
**Update**
- PyTorch의 LSTM 모델을 이용하여 서울특별시 중구의 2017 ~ 2019년 까지의 대기오염물질 중 오존농도 예측.

**to fix**
- coefficient correlation NAN으로 나옴 <- ..?
- 데이터 전처리 중 결측치 처리 과정에서 결측치가 있다면 해당 timestamp 데이터 아묻따 제거해버려서 예측결과에 약간 time shift oo,,
	-> 다른 방법 강구 필요,,
