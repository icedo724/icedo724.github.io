---
layout: cv
title: Projects
permalink: /projects/
---
<style>
  @import url('https://cdn.jsdelivr.net/gh/orioncactus/pretendard/dist/web/static/pretendard.css');
  body, h1, h2, h3, h4, h5, h6, p, li, a {
    font-family: 'Pretendard', -apple-system, BlinkMacSystemFont, system-ui, Roboto, 'Helvetica Neue', 'Segoe UI', 'Apple SD Gothic Neo', 'Noto Sans KR', sans-serif !important;
  }
  h2 {
    border-bottom: 2px solid #eaeaea;
    padding-bottom: 8px;
    margin-top: 2.5em;
    margin-bottom: 1em;
  }
  @media print {
    body, h1, h2, h3, h4, p, li, span {
      background-color: #fff !important;
      color: #000 !important;
    }

    a {
      text-decoration: underline !important;
      color: #000 !important;
    }

    h2, h3 {
      page-break-after: avoid;
    }
    li, p {
      page-break-inside: avoid;
    }

    * {
      box-shadow: none !important;
      text-shadow: none !important;
    }
  }
</style>
# 주요 프로젝트

## 실무 프로젝트

### 거래처 데이터 베이스 구축 및 분석
* 사내 거래처인 병원 데이터와 HIRA(건강보험심사평가원) 공공 데이터를 결합하여 데이터 분석 환경 구축.
* 구축된 데이터를 바탕으로 거래처 그룹별 카이제곱 검정을 수행하여 핵심 영업 요인 및 고객 세분화 인사이트 도출.
* 🔗 [GitHub](https://github.com/icedo724/medi) | 📝 [리포트](https://www.notion.so/miniminimin/2e0fbcdaed2880f1a37fe87f58603c1a?source=copy_link)

## 개인 프로젝트

### 리그오브레전드 상위 플레이어 메타 대시보드 구축
* Riot Games API를 활용하여 상위 티어 플레이어들의 플레이 데이터를 수집.
* 챔피언 픽률, 아이템 트리, 승률 간의 상관관계를 통계적으로 분석하여 게임 내 최적의 메타 인사이트 도출.
* 🔗 [GitHub](https://github.com/icedo724/LoL-DashBoard) | 📊 [대시보드](https://lolhighplayer.streamlit.app/)

### 로스트아크 경제 시계열 분석
* 로스트아크 거래소 데이터를 수집하여 게임 내 경제 흐름에 대한 시계열 분석 수행.
* 게임 내 정기적/비정기적 이벤트 요인이 경제 타격에 미치는 영향을 파악하고, 시계열 예측 모델을 적합시켜 요인 분석. 
* 분석 결과를 누구나 쉽게 확인할 수 있도록 Streamlit 기반 인터랙티브 대시보드 배포.
* 🔗 [GitHub](https://github.com/icedo724/LoaQuant) | 📝 [리포트](https://www.notion.so/miniminimin/318fbcdaed2880cd8de8dd88406d3564?source=copy_link) | 📊 [대시보드](https://loaquant.streamlit.app/)

### 메이플스토리 고레벨 유저 경험치 분석
* 고레벨 유저의 경험치 변동에 영향을 미치는 요인 검정
* 🔗 [GitHub](https://github.com/icedo724/Maplestory_Exp_Analysis) | 📝 [리포트](https://www.notion.so/miniminimin/32afbcdaed288075a929eb7f533361b0?source=copy_link) | 📊 [대시보드](https://maple-exp-analysis.streamlit.app/)

### 로스트아크 직업 밸런스 기반 유저 감성 분석
* '로스트아크 인벤' 직업 게시판 텍스트 데이터를 크롤링하여 패치 전후의 유저 여론 파악.
* 텍스트 라벨링 및 자연어 처리 기반의 감성 분석 모델 학습 진행.
* 🔗 [GitHub](https://github.com/icedo724/loabal)

### 월드 오브 워크래프트 한밤 경제 분석
* 사전 도메인 지식이 없는 새로운 환경의 데이터를 수집 및 분석.
* 기존 로스트아크 분석 프레임워크를 적용하여, 데이터 자체의 패턴과 흐름만으로 유의미한 경제적 인사이트를 도출.
* 🔗 [GitHub](https://github.com/icedo724/WoW-Auction) | 📝 [리포트](https://www.notion.so/miniminimin/32bfbcdaed288053bcfef33ce58e2d14?source=copy_link) | 📊 [대시보드](https://wowauction.streamlit.app/)

### 리그오브레전드 패치 예측 모델 
* 마스터 티어 이상 유저들의 패치별 매치 로그를 API로 대량 수집 및 전처리.
* 포지션, 승률, 픽률, 밴률 등의 변수를 활용하여 다음 패치의 챔피언 밸런스 조정(버프/너프) 방향을 예측하는 모델 구축.
* 🔗 [GitHub](https://github.com/icedo724/Loracle)

## 공모전 및 기타 저장소

### 제6회 교육 공공데이터 분석·활용대회
* 서울특별시 특수유아 분포와 특수교사 배치 현황 간의 불균등을 검증하기 위해 다중 회귀 모델링 수행 및 정책적 개선안 도출.
* 🔗 [GitHub](https://github.com/icedo724/Public-Education-Data) | 📝 [리포트](https://docs.google.com/document/d/17iBYTxN1GDq42raatcBSh5Tb9tC_8mGz_eF8uHsLi4Y/edit?usp=sharing)

### 제6회 서울교육 데이터 분석·활용 공모전
* 특수교육 대상자와 교육 가능 기관의 공간적 분포를 분석하여, 데이터 기반의 최적의 신규 특수학교 설립 방안 제안.
* 🔗 [GitHub](https://github.com/icedo724/Seoul-Edu) | 📝 [리포트](https://docs.google.com/document/d/1fW1vxKnGjlf3FzR50H1fesZoMP0e5QDs-lg9OM7gIJQ/edit?usp=sharing)

### Kaggle Competitions
* Kaggle을 활용한 머신러닝/데이터 분석 대회 참여 및 코드 기록.
* 🔗 [GitHub](https://github.com/icedo724/KaggleCompetition)