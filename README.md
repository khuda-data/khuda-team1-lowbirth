# 출산율과 주거지표 분석 프로젝트

## 프로젝트 개요
이 프로젝트는 광역지자체별로 주거지표(PIR, 전세가율, 공공임대비율)가 출산율에 미치는 영향을 분석하고 시각화합니다.

## 분석 내용
1. 데이터 전처리
   - 지역별 데이터 그룹화
   - 필요한 컬럼: 지역명, 출산율, PIR, 전세가율, 공공임대비율

2. 지역별 회귀분석
   - 독립변수: PIR, 전세가율, 공공임대비율
   - 종속변수: 출산율
   - 각 지역별 최영향 변수 도출

3. 시각화
   - 전체 지역의 최영향 변수 분포 (countplot)
   - 지역별 최영향 변수 비교 (stripplot)

## 설치 및 실행 방법
1. 필요한 패키지 설치:
```bash
pip install -r requirements.txt
```

2. 분석 실행:
```bash
python housing_birthrate_analysis.py
```

## 결과물
- `most_influential_variables.png`: 전체 지역의 최영향 변수 분포
- `region_specific_influence.png`: 지역별 최영향 변수 비교
- `region_analysis_results.csv`: 상세 분석 결과
