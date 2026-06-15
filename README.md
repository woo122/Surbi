---

## 데이터 파일 (별도 공유)

`data/raw/` 폴더에 아래 파일을 직접 넣어주세요.

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

```bash
pip install pandas scikit-learn xgboost lightgbm joblib shap
```

---

## Git 사용법

### 처음 클론할 때
```bash
git clone https://github.com/woo122/Surbi.git
```

### 작업 후 올릴 때
```bash
git add .
git commit -m "작업 내용 간단히 작성"
git push
```

### 최신 내용 받아올 때
```bash
git pull
```

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