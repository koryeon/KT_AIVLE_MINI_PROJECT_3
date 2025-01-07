# KT_AIVLE_MINI_PROJECT_3

# 스마트폰 센서 기반 데이터를 활용한 행동 인식

이 프로젝트는 스마트폰의 가속도 및 자이로스코프 센서를 활용하여 인간 행동을 인식하는 기술(HAR; Human Activity Recognition)을 구현하는 것을 목표로 합니다. 이를 통해 동작을 분류하는 모델을 완성하고, 일반인을 대상으로 제공할 수 있는 연계 서비스를 구상합니다.


## 프로젝트 정보

- **주제**: 스마트폰 센서 기반 데이터를 활용한 행동 인식
- **사전 학습 과목**: 데이터 처리, 데이터 분석, 딥러닝 모델링
- **데이터 출처**: [UCI Machine Learning Repository - Human Activity Recognition Using Smartphones](https://archive.ics.uci.edu/ml/datasets/human+activity+recognition+using+smartphones)
- **데이터 유형**: Tabular
- **문제 유형**: Classification


## 인간 행동 인식 (HAR)란?

인간 행동 인식(HAR)은 다양한 센서를 활용하여 사람의 모션이나 제스처와 관련된 정보를 수집하고 해석하여 행동을 인식하는 기술입니다. 

### 주요 센서

#### Accelerometer (가속도 센서)
- 물체의 선형 가속도를 측정하는 센서입니다.
- 예시: 일정 시간 동안 X, Y, Z 축으로 얼마나 빠르게 움직였는가?

#### Gyroscope (자이로스코프 센서)
- 물체의 각속도를 측정하는 센서입니다.
- 예시: 일정 시간 동안 X, Y, Z 축으로 각도가 얼마나 변했는가?

<img width="423" alt="스크린샷 2025-01-07 오후 7 56 31" src="https://github.com/user-attachments/assets/556412d8-177c-47f2-8c7b-7021ffa6383a" />



## 프로젝트 주요 단계
<img width="541" alt="스크린샷 2025-01-07 오후 7 57 12" src="https://github.com/user-attachments/assets/d89cb7eb-d841-4d56-b8da-3b09432a52c3" />
<img width="541" alt="스크린샷 2025-01-07 오후 7 57 58" src="https://github.com/user-attachments/assets/2f4b7e07-3a03-4fb4-a7db-12579fde1b6f" />

### 1. 데이터 탐색 (EDA)

주어진 데이터의 구성 및 분포를 확인하고, 분류 문제 해결에 유의미한 feature 및 label 변수를 탐색적으로 분석합니다.

#### 주요 활동
- 기본 정보 확인하기
- 변수별 중요도 확인하기
- 그룹별 중요도 확인하기
- 일부 변수의 실제값 분포 확인하기


### 2. 기본 모델링

중요도 상위의 변수를 활용하여 여러 알고리즘으로 target 변수를 분류하는 모델을 생성하고 평가합니다.

#### 주요 활동
- 데이터 준비하기
- 다양한 알고리즘으로 분류 모델 생성하기
- 하이퍼파라미터 튜닝하기
- 성능 비교하기


### 3. 단계별 모델링 및 파이프라인 구축

#### 단계 1: 정적/동적 행동 분류
- 6개의 행동을 정적/동적으로 나누고, 두 그룹을 분류하는 모델을 생성합니다.

#### 단계 2: 세부 동작 분류
- 정적 행동(3가지)과 동적 행동(3가지)에 대해 각각 분류 모델을 생성합니다.

#### 모델 통합
- 단계별 모델을 통합하고 최종 예측 결과와 성능 평가가 나오도록 구성합니다.

<img width="600" alt="스크린샷 2025-01-07 오후 7 49 57" src="https://github.com/user-attachments/assets/0064b97f-7b15-4a8f-86f6-5fd5b9ead3f8" />


## 첨부 자료
- 센서 데이터 설명 이미지
- 단계별 모델링 프로세스 이미지
