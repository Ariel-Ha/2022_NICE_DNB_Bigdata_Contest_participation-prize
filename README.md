# 2022_NICE_DNB_Bigdata_Contest_participation-prize
2022 (주) NICE DNB 비재무 데이터를 활용한 중소기업 휴폐업 예측 챌린지 장려상 수상작 
# 중소기업 휴폐업 예측 챌린지
---
## Project Overview
- 팀명 : 골목대장
- 팀원 : [김홍범](https://github.com/billkim418) - 1대장, [이태영](https://github.com/epzlfnql) - 2대장, [하연진](https://github.com/YeonJin55) - 3대장
- 분석 목적 : 미시경제, 거시경제, 인적자원 관점의 다양한 파생변수를 기반으로 중소기업의 휴폐업을 예측하고 유의미한 지표를 발굴하며 최적화된 휴폐업 예측 모델 개발을 목적으로 함
- 데이터 : 재무 데이터(NICE DNB 제공) + 비재무 데이터(크롤링을 통한 수집)
## Project flow
1. 프로젝트 개요
- 프로젝트 목적
- 배경 및 필요성
2. 데이터 수집 및 전처리
- 미시 경제 지표
- 거시 경제 지표
- Baseline 전처리 지표
3. 분석 모형
- 데이터 불균형 및 정규화
- 모델 선정
- 모델 결과 해석 - Feature importance
- 모델 결과 해석 - SHAP Value
4. 참고 문헌
## 최종 모델 예측 결과
- (CV = 10, StartifiedKfold 이용)

|Model|RandomForest|XGBoost|LightGBM|CATBoost|ANN|
|:---:|:---:|:---:|:---:|:---:|:---:|
|Accuracy|0.966|**0.966**|0.965|0.964|0.940|
|Recall|0.974|**0.974**|0.978|0.974|0.961|
|Precision|0.961|**0.961**|0.956|0.958|0.929|
|AUPRC|0.948|**0.948**|0.945|0.946|0.911|
|F1_Score|0.966|**0.966**|0.965|0.964|0.940|
|AUROC|0.998|**0.998**|0.965|0.998|0.992|
## 발표 후 Feedback
- 비재무 데이터 수집 방법 미숙 -> 주어진 데이터는 굉장히 구체적으로 기업들의 특징이 기재되어 있었는데 이를 이용하여 일대일 매칭의 비재무 데이터를 수집했으면 더 좋은 결과를 보여줬을 것으로 생각되어짐
- 비재무 데이터 활용 방안 부족 -> 해당 모델을 활용하여 구체적인 방향성을 제시한 팀이 좋은 점수를 받았음
- ESG 데이터 활용성 -> 우리 팀같은 경우 ESG 데이터를 계획 단계에서 사용하지 않기로 결정하였는데, 해당 데이터를 중소 기업에 맞게끔 변형할수 있는 방안이 존재하였음
### [최종 보고서(pdf)](https://github.com/billkim418/Numble_Comepetitions/blob/main/ppt/%5BNICE%20DNB%5D%20%EC%B5%9C%EC%A2%85%EB%B0%9C%ED%91%9C%EC%9E%90%EB%A3%8C_%EA%B3%A8%EB%AA%A9%EB%8C%80%EC%9E%A5.pdf) 
### [최종 ppt](https://github.com/billkim418/Numble_Comepetitions/blob/main/ppt/%5BNICE%20DNB%5D%20%EC%B5%9C%EC%A2%85%EB%B0%9C%ED%91%9C%EC%9E%90%EB%A3%8C_%EA%B3%A8%EB%AA%A9%EB%8C%80%EC%9E%A5.pptx)
---
### 데이터의 경우 보안문제로 업로드 하지 않았음을 밝힙니다.
