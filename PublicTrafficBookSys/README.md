<div align="center">
<h1>통합 교통 예매 시스템</h1>
</div>

## 📝 소개
C언어로 구현한 콘솔 기반 통합 교통 예매 시스템입니다.
열차, 버스, 배, 비행기 4가지 교통수단의 예매를 하나의 인터페이스에서 처리합니다.

<br />

## 📂 프로젝트 구조
```
PublicTrafficBookSys/
├── main.c              # 메인 진입점 (교통수단 선택 메뉴)
├── train_func.c        # 열차 예매 기능
├── train_header.h      # 열차 헤더
├── bus_func.c          # 버스 예매 기능
├── bus_header.h        # 버스 헤더
├── ship_func.c         # 배 예매 기능
├── ship_header.h       # 배 헤더
├── planeFunc.c         # 비행기 예매 기능
├── airplane.h          # 비행기 헤더
└── PublicTrafficBookSys.vcxproj    # Visual Studio 프로젝트
```

<br />

## ⚙ 기술 스택
<div>
<img src="https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=white"/>
<img src="https://img.shields.io/badge/Visual_Studio-5C2D91?style=for-the-badge&logo=visualstudio&logoColor=white"/>
</div>

<br />

## 🚉 지원 교통수단
| 교통수단 | 기능 |
|:---:|:---|
| 열차 | 노선 조회, 좌석 선택, 예매/취소 |
| 버스 | 노선 조회, 좌석 선택, 예매/취소 |
| 배 | 항로 조회, 좌석 선택, 예매/취소 |
| 비행기 | 항공편 조회, 좌석 선택, 예매/취소 |

<br />

## 🖥️ 실행 방법
Visual Studio에서 프로젝트를 열고 빌드 후 실행합니다.
```
1. 교통수단 선택 (열차/버스/배/비행기)
2. 노선 및 일정 조회
3. 좌석 선택 및 예매 확정
```
