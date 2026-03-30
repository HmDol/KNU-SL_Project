<div align="center">
<h1>전기차 시장 및 회생제동 분석</h1>
</div>

## 📝 소개
한국교통안전공단의 전기 화물차 센서 데이터를 분석하여
**배터리 효율**, **회생제동 성능**, **에어컨 영향** 등 전기차 운행 특성을 분석하는 프로젝트입니다.

<br />

## 📂 프로젝트 구조
```
PandasProject/
├── main.ipynb              # 전체 분석 노트북
├── EV_sensor_core.csv      # 전기차 핵심 센서 데이터
└── ev_sensor_values.csv    # 센서 원본 데이터
```

<br />

## ⚙ 기술 스택
<div>
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
<img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white"/>
<img src="https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge&logo=python&logoColor=white"/>
</div>

<br />

## 🔍 주요 분석 내용
| 분석 항목 | 결과 |
|:---:|:---|
| 회생제동 발생 비율 | 감속 중 58.76% |
| 브레이크-회생제동 연동 | 브레이크 ON 시 49.85% |
| 저속 회생전류 | 0~20 rpm 구간 평균 -15.75A |
| 에어컨 OFF 전비 | 3.28 km/kWh |
| 에어컨 ON 전비 | 2.95 km/kWh (약 10% 감소) |

<br />

## 📊 파이프라인
1. **데이터 로드** - 전기화물차 센서 27개 컬럼 데이터 로드
2. **회생제동 분석** - 감속/브레이크 구간 필터링 후 통계
3. **속도 구간별 분석** - RPM 구간별 회생전류 평균값
4. **에너지 효율 분석** - 에어컨 ON/OFF 조건별 전비 비교
5. **시각화** - 구간별 전력 소비 및 회생 패턴 시각화
