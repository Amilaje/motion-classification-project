# 스마트폰 센서 기반 모션 분류 프로젝트

## 개요
스마트폰 센서 데이터를 분석하여 사용자의 행동(걷기, 서기, 누워있기 등)을 분류하는 분류 모델을 구축합니다.  
KT Aivle School 과정 중 수행한 팀 프로젝트입니다.

## 프로젝트 구조
1. **탐색적 데이터 분석 (EDA)**  
   - 데이터 전반 파악  
   - feature 통계, 상관관계 시각화

2. **기본 모델링 (Baseline)**  
   - 기본 분류 모델(XGBoost, LightGBM) 적용  
   - Accuracy, Macro-F1 기반 성능 비교

3. **파이프라인 기반 고도화 모델링**  
   - ColumnTransformer + Pipeline을 통한 feature 엔지니어링 자동화  
   - 파라미터 튜닝 및 성능 개선

4. **딥러닝 모델링 (DNN)**  
   - TensorFlow 기반의 다층 퍼셉트론(MLP) 모델 구성  
   - 조기 종료(EarlyStopping), Dropout 등으로 성능 향상

## 🛠사용 기술
- Python, Pandas, Scikit-learn, TensorFlow
- XGBoost, LightGBM
- Jupyter Notebook, Google Colab
- EDA: matplotlib, seaborn

## 데이터 구성
- `data01_train.csv`: 훈련용 센서 데이터
- `data01_test.csv`: 테스트 데이터
- `features_description.xlsx`: Feature 이름 설명서

## 폴더 구조
├── data/ : 데이터 파일
├── notebooks/ : 분석 및 모델링 노트북
├── images/ : 시각화 결과
├── docs/ : 기획 및 문서 자료
├── requirements.txt: 패키지 목록
└── README.md : 프로젝트 소개 문서

## 성능 지표
- 주요 모델: XGBoost, LightGBM, DNN
- 최고 Macro-F1: **0.93 이상** (최종 모델 기준)

## 팀원
- 최진호, 이원준, 장우진, 이정훈, 최태환, 황지윤, 조하민, 정민기  
(KT Aivle School 팀 프로젝트)

## 주요 학습 내용
- 다양한 모델 간 비교를 통한 적합성 판단
- Pipeline, ColumnTransformer, GridSearchCV의 활용법
- 딥러닝 기반 모델과 전통 ML 모델 간 성능 비교
- 고차원 feature 처리 및 시각화 기법

