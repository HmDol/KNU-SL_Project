<div align="center">
<h1>배달 데이터를 통한 분석 및 인사이트 도출</h1>
</div>

## 📝 소개
한국교통안전공단의 배달 데이터와 기상 데이터를 결합하여
날씨 조건이 배달 주문량에 미치는 영향을 분석하는 프로젝트입니다.

<br />

## 📂 프로젝트 구조
```
DeliveryProject/
├── weather&delivery.ipynb  # 날씨-배달 상관관계 분석
└── Data/                   # 배달 및 기상 데이터
```

<br />

## ⚙ 기술 스택
<div>
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
<img src="https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge&logo=python&logoColor=white"/>
</div>

<br />

## 🔍 주요 내용
| 항목 | 내용 |
|:---:|:---|
| 데이터 | 한국교통안전공단 배달 데이터 (380,741건) |
| 분석 기간 | 2019년 7월 / 2020년 1월, 7월 |
| 기상 변수 | 강수형태, 강수량, 기온 |
| 음식 카테고리 | 한식, 분식, 카페, 치킨, 피자, 중식 등 14개 |

<br />

## 📊 주요 분석 결과
1. **계절별 TOP5** - 계절에 따른 인기 배달 품목 변화
2. **강수 영향** - 강수형태(맑음/비/눈)에 따른 주문량 차이
3. **태풍 영향** - 극단적 기상 상황의 배달 수요 분석
4. **기온 상관관계** - 기온 변화에 따른 음료/음식 카테고리별 반응
