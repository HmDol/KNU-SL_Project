<div align="center">
<h1>인물 이미지 분류기</h1>
</div>

## 📝 소개
UTKFace 데이터셋을 활용하여 얼굴 이미지에서 **연령대**, **성별**, **피부색**을 분류하는
머신러닝 파이프라인 프로젝트입니다. PCA 차원 축소와 Tkinter UI가 포함되어 있습니다.

<br />

## 📂 프로젝트 구조
```
Human_Divide/
├── 01_img_divide.ipynb         # 연령대별 이미지 분류 및 균형 샘플링
├── 02_img_to_csv.ipynb         # 이미지 → 픽셀 CSV 변환
├── 03_img_minist_pca.ipynb     # PCA 차원 축소 및 모델 학습
├── 04_confusion_matrix.ipynb   # 모델 성능 평가 (혼동 행렬)
├── 05_age_level_change.ipynb   # 연령대 레이블 재정의
├── Data/
│   ├── img_face_pca120_train.csv   # PCA 120차원 학습 데이터
│   └── img_face_pca120_test.csv    # PCA 120차원 테스트 데이터
├── Model/
│   ├── best_pipeline.joblib        # 최종 분류 모델
│   ├── pca_160.joblib              # PCA 변환기
│   ├── ageModel_pca160.joblib      # 연령대 분류 모델
│   ├── gender_model.jolib          # 성별 분류 모델
│   └── skincolor_model.joblib      # 피부색 분류 모델
└── UI/
    ├── inference.py                # 추론 로직
    └── ui.py                       # Tkinter GUI
```

<br />

## ⚙ 기술 스택
<div>
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white"/>
<img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
<img src="https://img.shields.io/badge/Tkinter-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
</div>

<br />

## 🔍 주요 내용
| 항목 | 내용 |
|:---:|:---|
| 데이터셋 | UTKFace (원본 23,709개 → 균형 샘플 2,562개) |
| 연령대 분류 | 7개 그룹 (영유아~고령) |
| 성별 균형 | 각 그룹 366개 (남 183, 여 183) |
| 차원 축소 | PCA 120~160 차원 |

<br />

## 📊 파이프라인
1. **이미지 분류** - UTKFace를 연령대별 폴더로 분류 및 균형 샘플링
2. **CSV 변환** - 이미지 픽셀을 CSV로 직렬화
3. **PCA 학습** - 차원 축소 후 분류 모델 학습
4. **추론 UI** - Tkinter GUI에서 이미지 업로드 → 결과 출력
