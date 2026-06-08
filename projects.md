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
  .project-problem {
    border-left: 3px solid #888;
    padding-left: 8px;
    margin: 4px 0 8px 0;
    font-size: 0.88em;
    line-height: 1.5;
  }
  .project-result {
    border-left: 3px solid #4a9eff;
    padding-left: 8px;
    margin: 4px 0 8px 0;
    font-size: 0.88em;
    line-height: 1.5;
  }
  .project-impact {
    border-left: 3px solid #2ecc71;
    padding-left: 8px;
    margin: 4px 0 12px 0;
    font-size: 0.88em;
    font-weight: 600;
    line-height: 1.5;
  }
  .badge-scale {
    background-color: rgba(74, 158, 255, 0.12);
    border: 1px solid rgba(74, 158, 255, 0.3);
    color: #4a9eff;
    padding: 2px 10px;
    border-radius: 12px;
    font-size: 0.72em;
    font-weight: 500;
  }
  .project-progress {
    margin: 6px 0 10px 0;
  }
  .progress-bar {
    height: 4px;
    background: var(--color-border);
    border-radius: 2px;
    margin: 4px 0;
  }
  .progress-fill {
    height: 100%;
    background: #4a9eff;
    border-radius: 2px;
  }
  .progress-label {
    font-size: 0.75em;
    opacity: 0.65;
    margin-right: 8px;
  }
  .progress-note {
    font-size: 0.75em;
    opacity: 0.65;
  }
  .badge-award {
    display: inline-block;
    font-size: 0.7em;
    font-weight: 700;
    padding: 2px 8px;
    border-radius: 10px;
    background-color: #fff8e1;
    color: #b8860b;
    vertical-align: middle;
    margin-left: 8px;
  }
  html[data-theme="dark"] .badge-award {
    background-color: #3d2e00;
    color: #f5c842;
  }
  .badge-entry {
    display: inline-block;
    font-size: 0.7em;
    font-weight: 600;
    padding: 2px 8px;
    border-radius: 10px;
    background-color: #e8f4e8;
    color: #2d6a2d;
    vertical-align: middle;
    margin-left: 8px;
  }
  html[data-theme="dark"] .badge-entry {
    background-color: #1a3a1a;
    color: #6fcf6f;
  }
  .badge-live {
    display: inline-flex;
    align-items: center;
    gap: 4px;
    font-size: 0.7em;
    font-weight: 600;
    padding: 2px 8px;
    border-radius: 10px;
    background-color: #e8f8ee;
    color: #1a7a40;
    vertical-align: middle;
    margin-left: 8px;
  }
  .badge-live::before {
    content: '';
    display: inline-block;
    width: 6px;
    height: 6px;
    border-radius: 50%;
    background-color: #2ecc71;
    animation: pulse-live 2s infinite;
    flex-shrink: 0;
  }
  @keyframes pulse-live {
    0%, 100% { opacity: 1; }
    50% { opacity: 0.3; }
  }
  html[data-theme="dark"] .badge-live {
    background-color: #0d2e1a;
    color: #4cda82;
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

<p style="font-size:0.85em; opacity:0.6; margin-top:-0.5em;">일부 대시보드는 Streamlit Cloud에서 슬립 상태일 수 있습니다.<br>접속 시 <strong>Yes, get this app back up!</strong> 버튼을 누르면 재시작됩니다.</p>

## 실무 프로젝트

<div class="project-card" id="project-medi">
<h3>거래처 데이터 보강 및 등급 재조정 방안 제시</h3>
<p class="project-impact">직관에 의존하던 거래처 등급을 정량 기준으로 전환 — 영업 우선순위 재편의 데이터 근거 마련</p>
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

### 로스트아크

<div class="project-card" id="project-loaquant">
<h3>로스트아크 경제 시계열 분석<span class="badge-live">Live</span></h3>
<p class="project-impact">재화 가격 변동 원인을 이벤트 단위로 분해, 다음 충격 규모를 미리 가늠할 수 있는 판단 기준 제공</p>
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
<h3>LOABAL - 로스트아크 커뮤니티 감정분석</h3>
<p class="project-impact">패치 전후 유저 감성 점수 시계열 시각화 → "이번 패치에 유저들이 어떻게 반응했는가"를 정량으로 제시</p>
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

### 메이플스토리

<div class="project-card">
<h3>메이플스토리 고레벨 유저 경험치 분석</h3>
<p class="project-impact">285레벨 이상 활성 유저 96,000명 실데이터로 신규 지역 공개·썬데이 메이플의 경험치 영향을 정량 측정</p>
<div class="project-tags">
  <span class="tag">Python</span>
  <span class="tag">Nexon API</span>
  <span class="tag">통계 검정</span>
</div>
<div class="project-links">
  <a class="project-link" href="https://github.com/icedo724/Maplestory_Analysis"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path></svg> GitHub</a>
  <a class="project-link" href="https://www.notion.so/miniminimin/32afbcdaed288075a929eb7f533361b0?source=copy_link"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path><polyline points="14 2 14 8 20 8"></polyline><line x1="16" y1="13" x2="8" y2="13"></line><line x1="16" y1="17" x2="8" y2="17"></line></svg> 리포트</a>
  <a class="project-link" href="https://maple-exp.streamlit.app/"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="18" y1="20" x2="18" y2="10"></line><line x1="12" y1="20" x2="12" y2="4"></line><line x1="6" y1="20" x2="6" y2="14"></line></svg> 대시보드</a>
</div>
</div>

<div class="project-card">
<h3>메이플스토리 유저 행동 클러스터링</h3>
<p class="project-impact">활동·성장 패턴 기반 유저 군집화 → 클러스터별 이탈 시점과 쇼케이스 반응 차이를 생존 분석으로 검증</p>
<div class="project-tags">
  <span class="tag">Python</span>
  <span class="tag">Nexon API</span>
  <span class="tag">클러스터링</span>
  <span class="tag">생존 분석</span>
</div>
<div class="project-links">
  <a class="project-link" href="https://github.com/icedo724/Maplestory_Analysis"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path></svg> GitHub</a>
  <a class="project-link" href="https://www.notion.so/miniminimin/346fbcdaed2880209e39ff1b490e34e5?source=copy_link"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path><polyline points="14 2 14 8 20 8"></polyline><line x1="16" y1="13" x2="8" y2="13"></line><line x1="16" y1="17" x2="8" y2="17"></line></svg> 리포트</a>
  <a class="project-link" href="https://maple-user-clustering.streamlit.app/"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="18" y1="20" x2="18" y2="10"></line><line x1="12" y1="20" x2="12" y2="4"></line><line x1="6" y1="20" x2="6" y2="14"></line></svg> 대시보드</a>
</div>
</div>

### 리그오브레전드

<div class="project-card">
<h3>리그오브레전드 상위 플레이어 메타 대시보드 구축</h3>
<p class="project-impact">마스터 이상 실데이터 기반 챔피언 픽률·승률 사분면 분류 — 메타 통계 서비스와 유사한 구조를 구현</p>
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
<h3>Loracle - 리그오브레전드 패치 예측 모델<span class="badge-wip">진행 중</span><span class="badge-wip">모델 버전: v7</span></h3>
<p class="project-impact">8패치 데이터로 분류·회귀 모델 v7 학습 완료 — 데이터 누적 시 패치 방향 예측 정확도 검증 예정</p>
<div class="project-progress">
  <span class="progress-label">진행률 약 38%</span>
  <div class="progress-bar"><div class="progress-fill" style="width: 38%"></div></div>
  <span class="progress-note">현재: 9패치분 수집 완료 · 목표 24패치 (1년치)</span>
</div>
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

### 월드 오브 워크래프트


<div class="project-card">
<h3>월드 오브 워크래프트 한밤 경제 분석<span class="badge-live">Live</span></h3>
<p class="project-impact">신규 확장팩 '한밤'에 따른 경제 변동 분석 및 로스트아크 분석 프레임워크의 이식 가능성 확인</p>
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

### 배틀그라운드

<div class="project-card">
<h3>배틀그라운드 유저 클러스터링</h3>
<p class="project-impact">유저 6,759명을 행동 패턴 4개 세그먼트로 분류 — 세그먼트별 독립 KPI 설계로 A/B 실험 정밀도를 높이는 프레임워크 구축</p>
<div class="project-tags">
  <span class="tag">Python</span>
  <span class="tag">PUBG API</span>
  <span class="tag">클러스터링</span>
  <span class="tag">PCA</span>
  <span class="tag">A/B 테스트</span>
</div>
<div class="project-links">
  <a class="project-link" href="https://github.com/icedo724/pubg_clustering"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path></svg> GitHub</a>
  <a class="project-link" href="https://www.notion.so/miniminimin/PUBG-344fbcdaed2880908668fb1db24185c1?source=copy_link"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path><polyline points="14 2 14 8 20 8"></polyline><line x1="16" y1="13" x2="8" y2="13"></line><line x1="16" y1="17" x2="8" y2="17"></line></svg> 리포트</a>
</div>
</div>

### 붉은사막

<div class="project-card">
<h3>붉은사막 Steam 리뷰 분석</h3>
<p class="project-impact">출시 후 6주 만족도 추세를 외부 AAA 출시작 2종(Elden Ring·Cyberpunk 2077)과 정량 비교 — 핫픽스 시점 효과를 시계열 회귀로 입증</p>
<div class="project-tags">
  <span class="tag">Python</span>
  <span class="tag">Steam API</span>
  <span class="tag">NLP</span>
  <span class="tag">시계열 회귀</span>
  <span class="tag">통계 검정</span>
</div>
<div class="project-links">
  <a class="project-link" href="https://github.com/icedo724/crimson_desert_review"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path></svg> GitHub</a>
  <a class="project-link" href="https://www.notion.so/miniminimin/358fbcdaed28804e92f6c73ecc6fa899?source=copy_link"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path><polyline points="14 2 14 8 20 8"></polyline><line x1="16" y1="13" x2="8" y2="13"></line><line x1="16" y1="17" x2="8" y2="17"></line></svg> 리포트</a>
</div>
</div>

### 게임 외


<div class="project-card" id="project-jobsonar">
<h3>JobSonar - 데이터직군 채용공고 수집 및 조회 서비스<span class="badge-live">Live</span></h3>
<p class="project-impact">데이터직군 채용공고 자동 수집 → 직무·기술 스택 빈도 시각화 — 취업 시장 트렌드를 한 페이지에 집약</p>
<div class="project-tags">
  <span class="tag">Python</span>
  <span class="tag">SQL</span>
  <span class="tag">SQLite</span>
  <span class="tag">Web Crawling</span>
  <span class="tag">Dash</span>
</div>
<div class="project-links">
  <a class="project-link" href="https://github.com/icedo724/JobSonar"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path></svg> GitHub</a>
</div>
</div>

<div class="project-card" id="project-kbo-bayes">
<h3>KBO 베이지안 타율·진출확률 추정<span class="badge-live">Live</span></h3>
<p class="project-impact">시즌 초 타율의 평균회귀를 베이지안 shrinkage로 보정하는 추론 시스템 — 매일 자동 수집·갱신되며, 5개 시즌(2021–2025) walk-forward로 보정 없는 관측 타율(베이스라인) 대비 일관된 우월성을 검증</p>
<div class="project-tags">
  <span class="tag">Python</span>
  <span class="tag">베이지안</span>
  <span class="tag">Beta-Binomial</span>
  <span class="tag">Supabase</span>
  <span class="tag">GitHub Actions</span>
  <span class="tag">Next.js</span>
</div>
<div class="project-links">
  <a class="project-link" href="https://github.com/icedo724/kbo-bayes"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path></svg> GitHub</a>
  <a class="project-link" href="https://kbo-bayes.vercel.app"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="18" y1="20" x2="18" y2="10"></line><line x1="12" y1="20" x2="12" y2="4"></line><line x1="6" y1="20" x2="6" y2="14"></line></svg> 대시보드</a>
</div>
</div>