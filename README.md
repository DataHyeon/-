## Title : 로스만 상점매출 예측 모델링

<br>

### Author : DataHyeon

<br>

### Date : 22.12.19

<br>

### Language : Jupyter

<br>

### Dec

- 로스만 상점매출 데이터를 이용한 매출 예측 ML 모델링

<br>

### Module

- 전처리 : pandas, numpy
 
- 시각화 : matplotlib
 
- ML : xgboost, crossvalidation, sklearn

<br>

### File

- Main : main.ipynb

- Input : train.csv, test.csv, store.csv

- Ouput : submission.csv, submission2.csv

<br>

### Conclusion

- xgboost를 통한 Basic 모델 생성, K-Fold를 이용한 교차검증으로 기존 변수 2개만을 이용했을 때 mse가 가장 낮음

- 2개 변수로는 과적합의 문제가 있어 새로운 변수를 store.csv를 활용하여 FE를 통해 새로운 변수 생성

- FE를 통해 전처리된 총 24개의 데이터 변수로 교차검증을 진행하고 유의미한 17개의 변수로 학습

- 분석과 모델링을 통해 상점의 매출을 증가시키기 위해서는 프로모션 진행여부와 상점의 종류, 경쟁상점과의 거리, 특정달마다의 프로모션 등이 영향을 주는 것을 확인
