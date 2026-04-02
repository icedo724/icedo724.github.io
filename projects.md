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
    border-bottom: 2px solid var(--color-border);
    padding-bottom: 8px;
    margin-top: 2.5em;
    margin-bottom: 1em;
  }
  h3 {
    text-transform: none;
  }
  .project-card {
    border: 1px solid var(--color-border);
    border-radius: 10px;
    padding: 1.2em 1.5em;
    margin-bottom: 1.2em;
  }
  .project-card h3 {
    margin: 0 0 0.6em 0;
    font-size: 1em;
    font-weight: 600;
    text-transform: none;
  }
  .project-card ul {
    margin: 0 0 0.8em 0;
    padding-left: 1.2em;
  }
  .project-card li {
    margin-bottom: 0.3em;
    font-size: 0.9em;
    line-height: 1.5;
  }
  .project-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 6px;
    margin-bottom: 0.8em;
  }
  .tag {
    background-color: var(--color-border);
    color: var(--color-text);
    padding: 2px 10px;
    border-radius: 12px;
    font-size: 0.75em;
    font-weight: 500;
  }
  .project-links {
    display: flex;
    flex-wrap: wrap;
    gap: 14px;
  }
  .project-link {
    display: inline-flex;
    align-items: center;
    gap: 4px;
    font-size: 0.85em;
  }
  .badge-wip {
    display: inline-block;
    font-size: 0.7em;
    font-weight: 600;
    padding: 2px 8px;
    border-radius: 10px;
    background-color: #fff3cd;
    color: #856404;
    vertical-align: middle;
    margin-left: 8px;
  }
  html[data-theme="dark"] .badge-wip {
    background-color: #3d2e00;
    color: #ffc107;
  }
  .project-link svg path,
  .project-link svg circle,
  .project-link svg polyline,
  .project-link svg line,
  .project-link svg rect {
    stroke: currentColor;
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
    .project-card {
      page-break-inside: avoid;
      border-color: #ccc !important;
    }
    * {
      box-shadow: none !important;
      text-shadow: none !important;
    }
  }
</style>

# 주요 프로젝트

## 실무 프로젝트

<div class="project-card">
<h3>거래처 데이터 보강 및 등급 재조정 방안 제시</h3>
<ul>
  <li>건강보험 요양기관 공공데이터를 요양기호 기준으로 연동, API 호출 구조 기반 스키마 분리 설계안 제시.</li>
  <li>2년간 거래 이력에 ABC·RFM 분석을 적용해 기존 등급 체계를 정량 지표 기반으로 재분류.</li>
  <li>카이제곱 검정으로 등급 간 요인 유의성 검증, 방안의 통계적 타당성 확보</li>
</ul>
<div class="project-tags">
  <span class="tag">Python</span>
  <span class="tag">SQL</span>
  <span class="tag">카이제곱 검정</span>
</div>
<div class="project-links">
  <a class="project-link" href="https://github.com/icedo724/medi"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path></svg> GitHub</a>
  <a class="project-link" href="https://www.notion.so/miniminimin/2e0fbcdaed2880f1a37fe87f58603c1a?source=copy_link"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path><polyline points="14 2 14 8 20 8"></polyline><line x1="16" y1="13" x2="8" y2="13"></line><line x1="16" y1="17" x2="8" y2="17"></line></svg> 리포트</a>
</div>
</div>

## 개인 프로젝트

<div class="project-card">
<h3>리그오브레전드 상위 플레이어 메타 대시보드 구축</h3>
<ul>
  <li>Riot Games API를 활용하여 상위 티어 플레이어들의 플레이 데이터를 수집.</li>
  <li>챔피언 픽률, 아이템 트리, 승률 간의 상관관계를 통계적으로 분석하여 게임 내 최적의 메타 인사이트 도출.</li>
</ul>
<div class="project-tags">
  <span class="tag">Python</span>
  <span class="tag">Riot API</span>
  <span class="tag">통계 검정</span>
</div>
<div class="project-links">
  <a class="project-link" href="https://github.com/icedo724/LoL-DashBoard"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path></svg> GitHub</a>
  <a class="project-link" href="https://lolhighplayer.streamlit.app/"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="18" y1="20" x2="18" y2="10"></line><line x1="12" y1="20" x2="12" y2="4"></line><line x1="6" y1="20" x2="6" y2="14"></line></svg> 대시보드</a>
</div>
</div>

<div class="project-card">
<h3>로스트아크 경제 시계열 분석</h3>
<ul>
  <li>로스트아크 거래소 데이터를 수집하여 게임 내 경제 흐름에 대한 시계열 분석 수행.</li>
  <li>게임 내 정기적/비정기적 이벤트 요인이 경제 타격에 미치는 영향을 파악하고, 시계열 예측 모델을 적합시켜 요인 분석.</li>
  <li>분석 결과를 누구나 쉽게 확인할 수 있도록 Streamlit 기반 인터랙티브 대시보드 배포.</li>
</ul>
<div class="project-tags">
  <span class="tag">Python</span>
  <span class="tag">LostArk API</span>
  <span class="tag">시계열 분석</span>
</div>
<div class="project-links">
  <a class="project-link" href="https://github.com/icedo724/LoaQuant"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path></svg> GitHub</a>
  <a class="project-link" href="https://www.notion.so/miniminimin/318fbcdaed2880cd8de8dd88406d3564?source=copy_link"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path><polyline points="14 2 14 8 20 8"></polyline><line x1="16" y1="13" x2="8" y2="13"></line><line x1="16" y1="17" x2="8" y2="17"></line></svg> 리포트</a>
  <a class="project-link" href="https://loaquant.streamlit.app/"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="18" y1="20" x2="18" y2="10"></line><line x1="12" y1="20" x2="12" y2="4"></line><line x1="6" y1="20" x2="6" y2="14"></line></svg> 대시보드</a>
</div>
</div>

<div class="project-card">
<h3>메이플스토리 고레벨 유저 경험치 분석</h3>
<ul>
  <li>고레벨 유저의 경험치 변동에 영향을 미치는 요인 검정.</li>
</ul>
<div class="project-tags">
  <span class="tag">Python</span>
  <span class="tag">Nexon API</span>
  <span class="tag">통계 검정</span>
</div>
<div class="project-links">
  <a class="project-link" href="https://github.com/icedo724/Maplestory_Exp_Analysis"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path></svg> GitHub</a>
  <a class="project-link" href="https://www.notion.so/miniminimin/32afbcdaed288075a929eb7f533361b0?source=copy_link"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path><polyline points="14 2 14 8 20 8"></polyline><line x1="16" y1="13" x2="8" y2="13"></line><line x1="16" y1="17" x2="8" y2="17"></line></svg> 리포트</a>
  <a class="project-link" href="https://maple-exp-analysis.streamlit.app/"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="18" y1="20" x2="18" y2="10"></line><line x1="12" y1="20" x2="12" y2="4"></line><line x1="6" y1="20" x2="6" y2="14"></line></svg> 대시보드</a>
</div>
</div>

<div class="project-card">
<h3>LOABAL - 로스트아크 커뮤니티 감정분석 <span class="badge-wip">진행 중</span><span class="badge-wip">모델 버전: v2</span></h3>
<ul>
  <li>'로스트아크 인벤' 직업 게시판 텍스트 데이터를 크롤링하여 패치 전후의 유저 여론 파악.</li>
  <li>텍스트 라벨링 및 자연어 처리 기반의 감정 분석 모델 학습 진행.</li>
</ul>
<div class="project-tags">
  <span class="tag">Python</span>
  <span class="tag">Web Crawling</span>
  <span class="tag">NLP</span>
  <span class="tag">감정 분석</span>
</div>
<div class="project-links">
  <a class="project-link" href="https://github.com/icedo724/loabal"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path></svg> GitHub</a>
  <a class="project-link" href="https://www.notion.so/miniminimin/LOABAL-327fbcdaed28802fa544c1a4d081d356?source=copy_link"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path><polyline points="14 2 14 8 20 8"></polyline><line x1="16" y1="13" x2="8" y2="13"></line><line x1="16" y1="17" x2="8" y2="17"></line></svg> 리포트</a>
</div>
</div>

<div class="project-card">
<h3>월드 오브 워크래프트 한밤 경제 분석</h3>
<ul>
  <li>사전 도메인 지식이 없는 새로운 환경의 데이터를 수집 및 분석.</li>
  <li>기존 로스트아크 분석 프레임워크를 적용하여, 데이터 자체의 패턴과 흐름만으로 유의미한 경제적 인사이트를 도출.</li>
</ul>
<div class="project-tags">
  <span class="tag">Python</span>
  <span class="tag">World of Warcraft API</span>
  <span class="tag">통계 검정</span>
</div>
<div class="project-links">
  <a class="project-link" href="https://github.com/icedo724/WoW-Auction"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path></svg> GitHub</a>
  <a class="project-link" href="https://www.notion.so/miniminimin/32bfbcdaed288053bcfef33ce58e2d14?source=copy_link"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path><polyline points="14 2 14 8 20 8"></polyline><line x1="16" y1="13" x2="8" y2="13"></line><line x1="16" y1="17" x2="8" y2="17"></line></svg> 리포트</a>
  <a class="project-link" href="https://wowauction.streamlit.app/"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="18" y1="20" x2="18" y2="10"></line><line x1="12" y1="20" x2="12" y2="4"></line><line x1="6" y1="20" x2="6" y2="14"></line></svg> 대시보드</a>
</div>
</div>

<div class="project-card">
<h3>Loracle - 리그오브레전드 패치 예측 모델<span class="badge-wip">진행 중</span><span class="badge-wip">모델 버전: v5</span></h3>
<ul>
  <li>마스터 티어 이상 유저들의 패치별 매치 로그를 API로 대량 수집 및 전처리.</li>
  <li>포지션, 승률, 픽률, 밴률 등의 변수를 활용하여 다음 패치의 챔피언 밸런스 조정 방향을 예측하는 모델 구축.</li>
</ul>
<div class="project-tags">
  <span class="tag">Python</span>
  <span class="tag">Riot API</span>
  <span class="tag">회귀 모델</span>
  <span class="tag">분류 모델</span>
</div>
<div class="project-links">
  <a class="project-link" href="https://github.com/icedo724/Loracle"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path></svg> GitHub</a>
  <a class="project-link" href="https://www.notion.so/miniminimin/Loracle-32afbcdaed28807faab9f5c891532ffd?source=copy_link"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path><polyline points="14 2 14 8 20 8"></polyline><line x1="16" y1="13" x2="8" y2="13"></line><line x1="16" y1="17" x2="8" y2="17"></line></svg> 리포트</a>
</div>
</div>

## 공모전 및 기타 저장소

<div class="project-card">
<h3>제6회 교육 공공데이터 분석·활용대회</h3>
<ul>
  <li>서울특별시 특수유아 분포와 특수교사 배치 현황 간의 불균등을 검증하기 위해 다중 회귀 모델링 수행 및 정책적 개선안 도출.</li>
</ul>
<div class="project-tags">
  <span class="tag">Python</span>
  <span class="tag">SQL</span>
  <span class="tag">공공데이터</span>
</div>
<div class="project-links">
  <a class="project-link" href="https://github.com/icedo724/Public-Education-Data"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path></svg> GitHub</a>
  <a class="project-link" href="https://docs.google.com/document/d/17iBYTxN1GDq42raatcBSh5Tb9tC_8mGz_eF8uHsLi4Y/edit?usp=sharing"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path><polyline points="14 2 14 8 20 8"></polyline><line x1="16" y1="13" x2="8" y2="13"></line><line x1="16" y1="17" x2="8" y2="17"></line></svg> 리포트</a>
</div>
</div>

<div class="project-card">
<h3>제6회 서울교육 데이터 분석·활용 공모전</h3>
<ul>
  <li>특수교육 대상자와 교육 가능 기관의 공간적 분포를 분석하여, 데이터 기반의 최적의 신규 특수학교 설립 방안 제안.</li>
</ul>
<div class="project-tags">
  <span class="tag">Python</span>
  <span class="tag">SQL</span>
  <span class="tag">공공데이터</span>
</div>
<div class="project-links">
  <a class="project-link" href="https://github.com/icedo724/Seoul-Edu"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path></svg> GitHub</a>
  <a class="project-link" href="https://docs.google.com/document/d/1fW1vxKnGjlf3FzR50H1fesZoMP0e5QDs-lg9OM7gIJQ/edit?usp=sharing"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path><polyline points="14 2 14 8 20 8"></polyline><line x1="16" y1="13" x2="8" y2="13"></line><line x1="16" y1="17" x2="8" y2="17"></line></svg> 리포트</a>
</div>
</div>

<div class="project-card">
<h3>Kaggle Competitions</h3>
<ul>
  <li>Kaggle을 활용한 머신러닝/데이터 분석 대회 참여 및 코드 기록.</li>
</ul>
<div class="project-tags">
  <span class="tag">Python</span>
  <span class="tag">머신러닝</span>
</div>
<div class="project-links">
  <a class="project-link" href="https://github.com/icedo724/KaggleCompetition"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path></svg> GitHub</a>
</div>
</div>
