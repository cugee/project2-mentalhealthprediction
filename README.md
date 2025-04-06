# Project2
### Kaggle 데이터의 여러 변수를 활용한 정신 건강 예측


## Table of Contents
- [프로젝트 Description](#프로젝트_Description)
- [프로젝트 정보](#프로젝트_정보)
- [프로젝트 결과](#프로젝트_결과)
  

## 프로젝트 Description
- Name, Gender, Age, City, Working Professional or Student, Profession, Academic Pressure, Work Pressure, CGPA, Study Satisfaction, Job Saticfaction, Sleep Duration, Dietary Habits, Degree, Suicidal thonghts, Work/Study Hours, Financial Stress, Family History of Mental Illness 변수와 우울증의 상관성을 가지는지 여부를 판단
- train / test 을 통한 prediction 진행


## 프로젝트 정보
1) **프로젝트 사용 언어 및 환경**
   - 사용 언어: Python
   - 사용 환경: jupyter notebook
     
2) **프로젝트 언어 사용 방식**
   - Kaggle 에서 관련 데이터 수집
   - sklearn 라이브러리를 활용한 머신러닝 코드 작성 및 실행
3) **프로젝트 구성 절차**
   - Kaggle에서 수집한 자료를 원활한 분석을 위해 모두 수치화
   - 의미있는 변수로 만들기 위해 추가적인 범주화 등 진행
   - sklearn 라이브러리의 랜덤포레스트 도구를 활용하여 머신러닝 모델 생성
   - 정확도 추출 및 우울증 영향도 분석


## 프로젝트 결과
1) **코드 설명**
   - 패키지 호출 및 데이터 호출
   - train, test 데이터셋을 동일하게 EDA 진행
   - train, test 데이터셋에서 결합하고자 하는 값은 결합하고, 수치화에 어려움이 있는 칼럼은 제외
   - 각 칼럼의 NULL 값 비율 확인 후, NULL 값을 모두 치환
   - 공분산을 통한 관게성 확인
   - sklearn 라이브러리를 활용한 랜덤포레스트 머신러닝 모델 생성 (train, test 데이터셋 활용)
   - 각 변수에 대한 영향도 분석
     
2) **실행 결과**
   - 정확도 분석 결과 91.90% 정확도로 우울증을 맞춤
   - 정제된 변수 중 가장 큰 영향을 미치는 것은 나이임을 알 수 있음
