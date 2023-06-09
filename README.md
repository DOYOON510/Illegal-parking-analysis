# 강서구에서 발생하는 불법주정차 해소 방안을 위한 분석 및 예측
2022.02 ~ 2022.3 (2개월)
[강서구 공모전 보고서.pdf](https://github.com/DOYOON510/Illegal-Parking/files/11480656/default.pdf)

## 📗 목차
  - 👨🏻‍💻 담당업무
  - ✍️ 서론
  - 📑 프로젝트 내용
    - 데이터 전처리
    - 모델링
    - 불법주정차 개선방
  - 🏆 결과 및 성과
  - 💡 Insight

## 👨🏻‍💻 담당업무
- EDA
- 데이터 전처리
- 모델링

## ✍️ 서론
- - 강서구의 한눈에 보는 민원 빅데이터 지역별 현황의 분석 결과를 활용해 강서구에서 가장 많이 들어오는 민원은 불법주정차와 관련되어 있다는 것을 확인하였다.
- 매년 증가하는 자동차 수에 비해 강서구의 주차 공간은 한정되어 있어 불법주정차와 관련된 문제가 해마다 증가하고 있음을 확인하였다.
- **불법주정차와 관련된 문제가 증가하면서 주민들의 불만의 소리가 커지고 있으므로 불법주정차 문제를 줄이기 위한 대안을 마련하고자, 이와 관련된 분석과 예측**을 진행했다.
![image](https://github.com/DOYOON510/Illegal-Parking/assets/129147977/ed5d3d85-1dc7-4be8-a71c-beedd2ecb6a6)

## 📑 프로젝트 내용
### 1. 데이터 전처리

- 강서구의 불법주정차 단속현황, CCTV 개수, 차량 수 현황등 불법주정차와 관련된 데이터를 수집하여 데이터별 기간, 지역 통일

### 2. 통계분석 진행

- CCTV 개수와 불법주정차 단속건수, 자동차 등록수와 불법주정차 단속건수와 관련하여 2가지의 귀무가설 및 대립가설을 설정
- 통계분석을 진행하여 2가지 가설의 상관계수와 p-value 값을 도출
- 상관계수와 p-value 값을 도출해본 결과 p-value의 값이 각각 약 0.00000168, 0.029으로,  유의수준 *a* = 0.05보다 작으므로 귀무가설을 기각

![image](https://github.com/DOYOON510/Illegal-Parking/assets/129147977/df8d79de-f0bc-4d50-8f12-64cdc0b1802d)

![image](https://github.com/DOYOON510/Illegal-Parking/assets/129147977/15dc3abc-3796-4547-8038-a92a6dd89ae3)

- 단속건수가 CCTV 개수에 따라 영향을받고, 단속건수가 자동차 등록 수에 영향을 받는다는 결과 도출

### 3. 모델링

- 시계열 예측모델인 ARIMA, Prophet을 사용하여 2022년부터 2025년까지의 자동차 등록 대수 현황을 예측을 진행해본 결과, 페이스북에서 개발한 시계열 예측모델 Prophet을 최종모델로 선정
- 예측한 결과 2021년 자동차 등록대수를 유지하거나 증가할 것으로 결과가 도출됐으므로, 통계분석 결과에 따라 불법주정차의 단속건수 또한 유지 및 증가할 것으로 예상

![image](https://github.com/DOYOON510/Illegal-Parking/assets/129147977/133f7a7f-0315-4035-825a-95be3019c622)
![image](https://github.com/DOYOON510/Illegal-Parking/assets/129147977/95213091-e068-4d14-a5be-baa006e3636d)


## 🏆 결과 및 성과
- 면허를 소지한 200명을 대상으로 설문조사를 진행한 결과, 불법주정차 문자 알림서비스 및 주차장 관련 애플리케이션을 인지하고 있는 사람이 매우 적다는 결과를 확인
![image](https://github.com/DOYOON510/Illegal-Parking/assets/129147977/1872b5cd-ce8a-4c3d-8f74-5d5122b1f110)
- 단속건수에 비해 설치된 CCTV 개수가 적은 가양2동, 공항동을 포함한 5개의 지역에 CCTV증설의 필요성을 제안
![image](https://github.com/DOYOON510/Illegal-Parking/assets/129147977/e2cba725-3c91-496d-9e4b-9dfb3dc39d82)

- 기존 주정차 단속 문자알림 서비스의 개선방안을 제시
![image](https://github.com/DOYOON510/Illegal-Parking/assets/129147977/4278a70b-5a4b-4a23-8776-348c7420db00)


## 💡 Insight
- 귀무가설과 대립가설을 설정하여 통계분석을 진행하는 등, 통계분석에 대한 개념과 전체적인 과정을 경험하였음
- ARIMA와 Prophet과 같은 시계열 예측 모델을 사용하며 시계열 예측 모델에 관한 이해력을 향상시켰음
