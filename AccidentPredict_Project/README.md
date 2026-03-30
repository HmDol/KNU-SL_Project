<div align="center">
<h1>산업사고 피해 예측 모델</h1>
</div>

## 📝 소개
미국 OSHA(산업안전보건청) 사고 데이터를 기반으로 산업현장 사고의 피해 유형을 예측하는 머신러닝 모델입니다.
사고 환경 요인, 인적 요인, 작업 유형 등을 분석하여 사고 결과를 예측합니다.

<br />

## 📂 프로젝트 구조
```
AccidentPredict_Project/
├── test.ipynb                                      # 데이터 분석 및 모델 학습
├── OSHA HSE DATA_ALL ABSTRACTS 15-17_FINAL.csv     # OSHA 사고 원본 데이터 (2015-2017)
└── external_test_osha_synthetic.csv                # 외부 테스트 데이터
```

<br />

## ⚙ 기술 스택
<div>
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white"/>
<img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
</div>

<br />

## 🔍 주요 내용
| 항목 | 내용 |
|:---:|:---|
| 데이터 | OSHA 산업사고 데이터 (2015~2017) |
| 주요 피처 | 사고 유형, 환경 요인, 인적 요인, 작업 유형 |
| 전처리 | OneHotEncoding, LabelEncoding, 이상치 처리 |

<br />

## 📊 파이프라인
1. **데이터 로드** - OSHA 사고 기록 CSV 로드
2. **전처리** - 불필요한 컬럼 제거, 인코딩
3. **모델 학습** - 분류 모델 학습 및 피해 유형 예측
4. **평가** - 외부 테스트 데이터로 성능 검증
