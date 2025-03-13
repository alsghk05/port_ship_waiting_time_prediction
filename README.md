# 효율적인 항만 운영 시스템을 위한 기계학습 기반 항만 내 선박 대기시간 예측

- **2024.08.28 ~ 2024.12.30**
- 머신러닝을 활용한 항만 내 선박의 대기시간을 예측하는 알고리즘 개발

> **핵심 전략**
> 
> 1. **불필요한 연산 최소화** 
>     1. 다양한 Feature Selection 방법(SHAP, PCA)을 적용하여 모델 성능을 평가하고 최적의 Feature를 선택
>     2. 도메인 지식을 활용한 Feature Engineering을 수행하여 의미 있는 변수를 추가
> 2. **모델 성능 향상**
>     1. 경량 모델(LR, RR)과 복잡한 모델(XGBoost, LGBM, Stacking 등)을 비교하여 최적 모델 선정
>     2. 실제 모델 간 성능 차이가 유의미한지 통계분석(T-test, ANOVA)을 통해 검증
>     3. 하이퍼파라미터 튜닝(GA)을 활용해 성능 개선

### 1. 개발 배경

- 코로나 19 팬데믹 이후 아시아 항만들의 체선 체화 현상이 점차 심각해짐에 따라 현재 최대 수출 물류난을 겪고 있음
    - 싱가포르 항에서는 3일 - 5일 정도 외항에 대기하는 체선이 계속되고 있고, 화물적체가 심화되면서 항만 운영에 악영향을 미침
- 이를 해결하기 위한 항만 시설 확충은 시간이 오래 걸리고 비용이 많이 듦
- 따라서 항만 내 선박의 대기시간을 예측하는 알고리즘을 제안하여 항만 내 체선 현상을 더 효율적으로 개선하는 데 도움이 되고자 함

### 2. 기대 효과

- 예측된 선박 대기시간을 기준으로 하여 체선 현상에 미리 대비할 수 있으며, 선박 스케줄링을 효율적으로 개선 가능
- 예측 결과는 항만 관리자 뿐만 아니라 각 선박 운항자에게도 제공되어 항만의 서비스 만족도를 향상시킬 수 있을 것으로 기대됨

### 3. 아키텍쳐

데이터 수집 및 전처리 → Feature selection → 모델링(LR, RR, RFR, XGBR, LGBR, CBR, GBR, MLP, LSTM, Stacking) → 모델 학습 및 평가($RMSE$, $MAE$, $R^2$ $score$) → 하이퍼 파라미터 튜닝(GA)을 통한 최적화

### 4. 사용 기술

- Python, Feature selection(SHAP, PCA) Machine Learning (LR, RR, RFR, XGBR, LGBR, CBR, GBR, MLP, LSTM, Stacking)

### 5. 라이브러리

- Numpy, Pandas, Matplotlib, Seaborn, shap, sklearn, xgboost, lightgbm, catboost, deap

### 6. 개발 환경

- 언어 : Python 3.10.9
- OS : Window 11
- IDE : Jupyter Notebook, VS Code

<aside>


### **🚀성과**

- **효율적인 항만 운영 시스템을 위한 기계학습 기반 항만 내 선박 대기시간 예측** ([학술지 게재](https://www.dbpia.co.kr/journal/articleDetail?nodeId=NODE12025218&nodeId=NODE12025218&mobileYN=N&medaTypeCode=185005&isPDFSizeAllowed=true&locale=ko&foreignIpYn=N&articleTitle=%ED%9A%A8%EC%9C%A8%EC%A0%81%EC%9D%B8+%ED%95%AD%EB%A7%8C+%EC%9A%B4%EC%98%81+%EC%8B%9C%EC%8A%A4%ED%85%9C%EC%9D%84+%EC%9C%84%ED%95%9C+%EA%B8%B0%EA%B3%84%ED%95%99%EC%8A%B5+%EA%B8%B0%EB%B0%98+%ED%95%AD%EB%A7%8C+%EB%82%B4+%EC%84%A0%EB%B0%95+%EB%8C%80%EA%B8%B0%EC%8B%9C%EA%B0%84+%EC%98%88%EC%B8%A1&articleTitleEn=Machine+learning-based+port+ship+waiting+time+prediction+for+efficient+port+operation+system&voisId=VOIS00762287&voisName=%ED%95%9C%EA%B5%AD%EC%A0%95%EB%B3%B4%EA%B8%B0%EC%88%A0%ED%95%99%ED%9A%8C+2024%EB%85%84%EB%8F%84+%EC%B6%94%EA%B3%84%EC%A2%85%ED%95%A9%ED%95%99%EC%88%A0%EB%8C%80%ED%9A%8C+%EB%B0%8F+%EB%8C%80%ED%95%99%EC%83%9D%EB%85%BC%EB%AC%B8%EA%B2%BD%EC%A7%84%EB%8C%80%ED%9A%8C&voisCnt=561&language=ko_KR&hasTopBanner=true))
- **대학생 논문 경진대회 금상**
</aside>
