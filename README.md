# Surbi — ML 파트

AI 기반 공공형 창업 의사결정 지원 플랫폼 Surbi의 ML 파트 레포지토리입니다.

담당자: 곽현우

---

## 프로젝트 구조

surbi-ml/
├── data/
│   ├── raw/          # 원본 CSV 파일 (Git 미포함, 별도 공유)
│   └── processed/    # 전처리 완료 데이터
├── notebooks/
│   ├── 01_데이터탐색.ipynb
│   ├── 02_전처리_병합.ipynb
│   ├── 03_모델학습.ipynb
│   └── 04_점수화_SHAP.ipynb
├── models/           # 학습된 모델 파일 (Git 미포함)
└── README.md

---

## 데이터 파일 (별도 공유)

data/raw/ 폴더에 아래 파일을 직접 넣어주세요.

데이터 링크 https://drive.google.com/drive/folders/1GLCQGtrlre-97Y_A79MGtjy9wIJSmlAU?usp=sharing

| 파일명 | 설명 |
|--------|------|
| store_info.csv | 소상공인 상가정보 (경쟁업체 수) |
| estimated_sales.csv | 서울시 추정매출 (y1, 회귀 정답값) |
| closure_rate.csv | 폐업률 (y2, 분류 정답값) |
| rent_price.csv | 부동산원 임대료 |
| resident_population.csv | 서울시 생활인구 |
| working_population.csv | 직장인구 |
| subway_passengers.csv | 지하철 승하차 인원 |

---

## 환경 설정

pip install pandas scikit-learn xgboost lightgbm joblib shap

---

## Git 사용법

처음 클론할 때
git clone https://github.com/woo122/Surbi.git

작업 후 올릴 때
git add .
git commit -m "작업 내용 간단히 작성"
git push

최신 내용 받아올 때
git pull

---

## 점수 구성

| 항목 | 배점 | 담당 |
|------|------|------|
| 유동인구 지수 | 20점 | ML 파트 |
| 업종 소비력 | 20점 | ML 파트 |
| 경쟁 강도 | 15점 | ML 파트 |
| 접근성 | 10점 | ML 파트 |
| 운영 안정성 | 15점 | ML 파트 |
| 정책 지원 적합도 | 20점 | 백엔드 파트 |