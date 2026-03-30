<div align="center">
<h1>자동차 시장 분석 및 인사이트 도출</h1>
</div>

## 📝 소개
네이버 자동차 검색 페이지에서 국내외 주요 브랜드의 차량 제원 정보를 크롤링하고,
수집된 데이터를 분석하여 자동차 시장 인사이트를 도출하는 프로젝트입니다.

<br />

## 📂 프로젝트 구조
```
Crawling_Project/
├── crawling.ipynb          # 네이버 자동차 제원 크롤링
├── review_crawling.ipynb   # 자동차 리뷰 크롤링
├── data_processing.ipynb   # 데이터 전처리
├── data_analyze.ipynb      # 데이터 분석 및 시각화
├── detail.csv              # 차량 제원 데이터 (2,216개 모델)
├── total.csv               # 수집 원본 데이터
└── total2~4.csv            # 처리 단계별 데이터
```

<br />

## ⚙ 기술 스택
<div>
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/Selenium-43B02A?style=for-the-badge&logo=selenium&logoColor=white"/>
<img src="https://img.shields.io/badge/BeautifulSoup-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
</div>

<br />

## 🔍 주요 내용
| 항목 | 내용 |
|:---:|:---|
| 수집 대상 | 현대, 기아, 제네시스, 르노, 벤츠, BMW, 테슬라, 렉서스 |
| 수집 규모 | 2,216개 차량 모델 |
| 수집 항목 | 엔진, 연료, 가속성능, 배터리 용량 등 29개 제원 |
| 분석 내용 | 브랜드별 성능 비교, 전기차 시장 트렌드 |

<br />

## 📊 파이프라인
1. **크롤링** - Selenium으로 네이버 자동차 페이지 자동화 수집
2. **전처리** - 결측치 처리, 데이터 정제
3. **분석** - 브랜드별/연료별/가격대별 인사이트 도출
4. **시각화** - Matplotlib을 활용한 시각화
