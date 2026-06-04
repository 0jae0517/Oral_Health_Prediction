# 🦷 Cheer up(치아 업) Clinic  
### 데이터 기반 청소년 구강 건강 위험도 예측 및 개인 맞춤형 관리 플랫폼

> 청소년의 스마트폰 과의존, 수면 상태, 정신건강, 생활습관 데이터를 기반으로  
> 구강 건강 위험도를 예측하고 개인 맞춤형 관리 솔루션을 제공하는 Streamlit 기반 웹 서비스입니다.

<br/>

## 🔗 Project Links

| 구분 | 링크 |
|---|---|
| 발표자료 | [발표자료](https://drive.google.com/file/d/1j-8EbZOCZkepf_FD33XVYiCSTOmO44Tz/view?usp=sharing) |
| GitHub Repository | [Oral_Health_Prediction](https://github.com/0jae0517/Oral_Health_Prediction) |
| Streamlit Demo | [시연 영상](https://drive.google.com/file/d/1j-8EbZOCZkepf_FD33XVYiCSTOmO44Tz/view?usp=sharing) |

<br/>

---

## 1. Project Overview

본 프로젝트는 청소년의 구강 건강 문제를 조기에 파악하기 위해  
**스마트폰 과의존, 수면의 질, 정신건강, 생활습관 요인**을 활용하여  
구강 건강 위험도를 예측하는 AI 기반 헬스케어 서비스입니다.

단순히 예측 결과만 제공하는 것이 아니라, 사용자의 스마트폰 의존 수준과 구강 건강 위험도를 함께 고려하여  
**개인 맞춤형 행동 가이드**를 제공하는 것을 목표로 합니다.

<br/>

### 핵심 기능

- 청소년 구강 건강 위험도 예측
- 스마트폰 과의존 척도 기반 위험군 분류
- 수면 상태 및 스마트폰 사용 시간 반영
- 머신러닝 기반 구강 증상 발생 가능성 예측
- 예측 결과에 따른 개인 맞춤형 솔루션 제공
- EDA 기반 통계 예측지도 시각화

<br/>

---

## 2. Background & Problem

청소년의 스마트폰 사용 시간이 증가하면서 수면 부족, 정신건강 문제, 생활습관 불균형이 함께 나타나고 있습니다.  
이러한 요인들은 구강 건강 관리 습관에도 영향을 줄 수 있으며, 구강 증상 발생 가능성과도 관련될 수 있습니다.

기존의 구강 건강 관리는 사후 치료 중심인 경우가 많기 때문에,  
본 프로젝트에서는 데이터 기반 예측 모델을 통해 구강 건강 위험을 조기에 파악하고  
예방적 관리 행동을 유도하는 서비스를 기획했습니다.

<br/>

### 문제 정의

| 문제점 | 설명 |
|---|---|
| 청소년 스마트폰 과의존 증가 | 스마트폰 사용 시간이 길어지며 수면, 생활습관, 건강 관리에 부정적 영향 가능 |
| 구강 건강 관리 부족 | 증상이 발생한 이후 병원을 찾는 사후 관리 중심 |
| 개인별 위험도 파악 어려움 | 생활습관과 심리 요인을 종합적으로 고려한 예측 서비스 부족 |
| 예방 중심 솔루션 부족 | 위험도에 따른 맞춤형 행동 가이드 제공이 제한적 |

<br/>

---

## 3. Service Preview

### Main Page & Service Overview

<img src="assets/01_main_overview.png" width="100%"/>

<br/>

### Oral Health Risk Prediction Form

<img src="assets/02_prediction_form.png" width="100%"/>

<br/>

### Prediction Result

<img src="assets/03_prediction_result.png" width="100%"/>

<br/>

### Personalized Solution

<img src="assets/04_personal_solution.png" width="100%"/>

<br/>

### EDA Dashboard

<img src="assets/05_eda_dashboard.png" width="100%"/>

<br/>

---

## 4. System Flow

<img src="assets/06_systemflow.png" width="100%"/>

<br/>

### 전체 서비스 흐름

```text
청소년 건강행태 데이터 수집
        ↓
데이터 전처리 및 주요 변수 선택
        ↓
스마트폰 과의존, 수면, 정신건강, 생활습관 변수 분석
        ↓
EDA 및 통계 분석
        ↓
머신러닝 모델 학습 및 성능 비교
        ↓
최종 예측 모델 선정
        ↓
Streamlit 기반 구강 건강 위험도 예측 서비스 구현
        ↓
예측 결과 및 개인 맞춤형 관리 솔루션 제공
```

<br/>

---

## 5. Dataset

본 프로젝트에서는 청소년 건강행태 관련 데이터를 기반으로  
구강 건강 증상과 관련된 주요 생활습관 및 심리 요인을 분석했습니다.

<br/>

### 주요 활용 변수

| 구분 | 변수 예시 |
|---|---|
| 인구통계 정보 | 성별, 학교급, 학업성적, 경제수준 |
| 스마트폰 사용 정보 | 주중 스마트폰 사용 시간, 주말 스마트폰 사용 시간, 스마트폰 과의존 척도 |
| 수면 관련 정보 | 수면의 질, 피로 회복 정도 |
| 정신건강 정보 | 스트레스, 불안, 절망감, 자살 생각 여부 |
| 구강 건강 정보 | 구강 증상 경험 여부, 구강 건강 위험도 |

<br/>

### 데이터 활용 목적

- 청소년의 스마트폰 과의존 수준 파악
- 수면 및 정신건강 요인과 구강 건강의 관계 분석
- 구강 건강 위험도 예측 모델 학습
- 개인 맞춤형 관리 솔루션 제공 기준 설계

<br/>

---

## 6. Data Analysis

EDA를 통해 스마트폰 사용 시간, 수면 상태, 스마트폰 의존도와 구강 증상 경험 간의 관계를 시각적으로 확인했습니다.

<br/>

### 주요 분석 관점

| 분석 항목 | 목적 |
|---|---|
| 스마트폰 사용 시간별 구강 증상 비율 | 사용 시간이 증가할수록 구강 증상 경험률이 달라지는지 확인 |
| 주중/주말 스마트폰 사용 비교 | 평일과 주말 사용 패턴 차이 분석 |
| 스마트폰 의존군 비율 | 일반군과 위험군의 분포 확인 |
| 수면 상태와 구강 건강 관계 | 수면 부족 여부에 따른 구강 증상 차이 분석 |
| 복합 위험도 분석 | 스마트폰 의존도와 수면 상태를 함께 고려한 위험도 확인 |

<br/>

### EDA Dashboard

<img src="assets/05_eda_dashboard.png" width="100%"/>

<br/>

---

## 7. Modeling

본 프로젝트에서는 구강 건강 위험도 예측을 위해 여러 머신러닝 모델을 비교하고,  
예측 성능과 서비스 적용 가능성을 고려하여 최종 모델을 선정했습니다.

<br/>

### 모델링 과정

```text
데이터 로드
  ↓
결측치 및 이상치 처리
  ↓
범주형 변수 인코딩
  ↓
학습/검증 데이터 분리
  ↓
여러 머신러닝 모델 학습
  ↓
성능 지표 비교
  ↓
최종 모델 선정
  ↓
Streamlit 서비스 연동
```

<br/>

### 사용 모델

| 모델 | 설명 |
|---|---|
| Logistic Regression | 기준 모델로 활용 |
| Random Forest | 비선형 관계와 변수 중요도 확인 |
| XGBoost | 최종 예측 성능 개선을 위한 부스팅 모델 |

<br/>

### Model Performance

<img src="assets/07_roc.png" width="100%"/>

<br/>

> 모델별 정량 성능표는 추후 Accuracy, Precision, Recall, F1-score, ROC-AUC 기준으로 추가할 예정입니다.

<br/>

### 모델 선정 기준

본 프로젝트는 헬스케어 위험도 예측 서비스이기 때문에  
단순 정확도뿐만 아니라 위험군을 놓치지 않는 것이 중요합니다.

따라서 모델 평가는 다음 기준을 함께 고려했습니다.

- 구강 건강 위험군을 잘 탐지하는지
- Recall 성능이 충분한지
- 예측 결과를 서비스 화면에서 직관적으로 설명할 수 있는지
- 사용자 입력값 기반 실시간 예측에 적합한지

<br/>

---

## 8. Service Features

### 1. 스마트폰 과의존 이해하기

사용자가 스마트폰 과의존의 정의와 주요 현상, 청소년 진단 기준을 이해할 수 있도록 구성했습니다.

- 조절 실패
- 현저성
- 문제적 결과
- 일반군 / 잠재적 위험군 / 고위험군 기준 제공

<br/>

### 2. 구강 건강 위험도 예측

사용자가 기본 정보, 스마트폰 과의존 척도, 수면 상태, 스마트폰 사용 시간을 입력하면  
AI 모델이 구강 건강 위험도를 예측합니다.

<br/>

### 3. 예측 결과 제공

예측 결과 화면에서는 다음 정보를 제공합니다.

- 스마트폰 의존 점수
- 스마트폰 의존군 분류
- 구강 건강 위험도
- 구강 증상 발생 확률
- 진단 결과 요약

<br/>

### 4. 개인 맞춤형 솔루션

예측 결과에 따라 사용자에게 맞는 행동 가이드를 제공합니다.

| 분류 | 제공 솔루션 예시 |
|---|---|
| 일반군 | 건강 유지 솔루션 |
| 잠재적 위험군 | 스마트폰 사용 시간 점검, 구강 관리 습관 개선 |
| 고위험군 | 전문가 상담 권장, 디지털 디톡스, 정기 구강검진 안내 |

<br/>

### 5. 통계 예측지도

EDA 분석 결과를 기반으로 스마트폰 사용 시간, 수면 상태, 구강 증상 경험률 등을 시각화하여  
전체 데이터 관점에서 위험 요인을 확인할 수 있도록 구성했습니다.

<br/>

---

## 9. Tech Stack

### Language & Library

| 구분 | 기술 |
|---|---|
| Language | Python |
| Data Analysis | Pandas, NumPy |
| Visualization | Matplotlib, Plotly |
| Machine Learning | Scikit-learn, XGBoost |
| Web Framework | Streamlit |
| Model Save/Load | Joblib, Pickle |
| Version Control | Git, GitHub |

<br/>

### Development Environment

| 구분 | 내용 |
|---|---|
| OS | Windows |
| IDE | VS Code / Jupyter Notebook |
| Package Management | pip / conda |
| Collaboration | GitHub, Google Drive, Slack |

<br/>

---

## 10. Project Structure

```text
Oral_Health_Prediction/
├── app.py
├── train.py
├── requirements.txt
├── README.md
│
├── data/
│   ├── raw/
│   └── processed/
│
├── models/
│   ├── model_meta.json
│   └── saved_model_files
│
├── plots/
│   ├── roc_curve
│   ├── confusion_matrix
│   └── feature_importance
│
├── assets/
│   ├── 01_main_overview.png
│   ├── 02_prediction_form.png
│   ├── 03_prediction_result.png
│   ├── 04_personal_solution.png
│   ├── 05_eda_dashboard.png
│   ├── 06_systemflow.png
│   └── 07_roc.png
│
├── 01_Data_Preprocessing.ipynb
├── 02_Statistical_Analysis.ipynb
└── EDA.ipynb
```

<br/>

---

## 11. How to Run

### 1. Repository Clone

```bash
git clone https://github.com/0jae0517/Oral_Health_Prediction.git
cd Oral_Health_Prediction
```

<br/>

### 2. Install Requirements

```bash
pip install -r requirements.txt
```

<br/>

### 3. Run Streamlit App

```bash
streamlit run app.py
```

<br/>

---

## 12. Expected Effect

본 서비스는 청소년이 자신의 스마트폰 사용 습관과 구강 건강 위험도를 쉽게 확인할 수 있도록 돕습니다.  
또한 단순 예측에 그치지 않고, 사용자의 상태에 맞는 행동 가이드를 제공함으로써  
구강 건강 문제를 조기에 인식하고 예방적 관리로 이어질 수 있도록 설계되었습니다.

<br/>

### 기대 효과

| 구분 | 기대 효과 |
|---|---|
| 사용자 측면 | 자신의 구강 건강 위험도를 쉽게 확인 가능 |
| 예방 관리 측면 | 증상 발생 전 생활습관 개선 유도 |
| 데이터 분석 측면 | 스마트폰 사용, 수면, 정신건강과 구강 건강의 관계 확인 |
| 서비스 측면 | AI 예측 결과를 웹 서비스 형태로 제공 |

<br/>

---

## 13. Limitations & Future Work

### Limitations

- 설문 기반 데이터이므로 사용자의 응답 정확도에 영향을 받을 수 있음
- 실제 의료 진단이 아닌 구강 건강 위험도 예측 및 참고용 서비스임
- 데이터셋의 변수 범위 내에서만 예측 가능
- 외부 검증 데이터에 대한 추가 평가 필요

<br/>

### Future Work

- 실제 사용자 입력 데이터 누적을 통한 모델 개선
- 치과 방문 이력 및 구강검진 데이터 연계
- 사용자별 장기 추적 관리 기능 추가
- 모바일 환경 최적화
- 지역 기반 치과 정보 추천 기능 고도화

<br/>

---

## 14. My Role

| 역할 | 내용 |
|---|---|
| 데이터 전처리 | 분석에 필요한 변수 정리 및 전처리 |
| EDA | 스마트폰 사용, 수면, 구강 건강 관련 시각화 |
| 모델링 | 머신러닝 모델 학습 및 성능 비교 |
| 서비스 구현 | Streamlit 기반 예측 웹 서비스 개발 |
| 결과 해석 | 예측 결과와 맞춤형 솔루션 연결 |
| 문서화 | README 및 발표자료 구성 |

<br/>

---

## 15. Notice

본 프로젝트는 학습 및 포트폴리오 목적의 데이터 분석 프로젝트입니다.  
제공되는 예측 결과는 의료적 진단이 아니며, 실제 구강 건강 문제가 의심되는 경우 전문 의료기관의 상담이 필요합니다.