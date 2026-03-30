<div align="center">
<h1>AI vs Human 텍스트 분류</h1>
</div>

## 📝 소개
AI가 생성한 텍스트와 인간이 작성한 텍스트를 구분하는 이진 분류 모델입니다.
자기소개 텍스트 데이터를 수집하여 **KoBERT** 기반 분류기를 학습시켰습니다.

<br />

## 📂 프로젝트 구조
```
AIvsHUMAN_Project/
├── 01_data_prepare.ipynb       # 데이터 수집 및 전처리
├── 02_KoBERT_Linear.ipynb      # KoBERT 모델 학습 (최종)
├── Data/
│   ├── human_made.csv          # 인간 작성 자기소개 (81개)
│   ├── AI_made.csv             # AI 생성 자기소개 (82개)
│   ├── all.csv                 # 병합 데이터 (161개)
│   └── all_sentence.csv        # 문장 단위 분할 데이터
├── train_fold.csv              # 학습 데이터
└── val_fold.csv                # 검증 데이터
```

<br />

## ⚙ 기술 스택
<div>
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white"/>
<img src="https://img.shields.io/badge/HuggingFace-FFD21F?style=for-the-badge&logo=huggingface&logoColor=black"/>
<img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
</div>

<br />

## 🔍 주요 내용
| 항목 | 내용 |
|:---:|:---|
| 모델 | KoBERT + Linear Head |
| 분류 | Human(0) / AI(1) |
| 데이터 | 자기소개 텍스트 161개 샘플 |
| 전처리 | 문장 단위 분할, 노이즈 제거 |

<br />

## 📊 파이프라인
1. **데이터 수집** - 인간 작성 / AI 생성 자기소개 텍스트 수집
2. **전처리** - 문장 단위 분할 및 데이터 정제
3. **모델 학습** - KoBERT Fine-tuning (Linear Head)
4. **평가** - K-Fold 교차 검증
