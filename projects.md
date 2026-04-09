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

## 실무 프로젝트

<div class="project-card" id="project-medi">
<h3>거래처 데이터 보강 및 등급 재조정 방안 제시</h3>
<p class="project-problem"><strong>문제:</strong> 영업 담당자 직관에만 의존하던 거래처 등급 체계 — 정량 기준 없어 이의제기·갱신 불가</p>
<p class="project-result"><strong>결과:</strong> 건강보험 공공데이터 3종 + 내부 2년 거래 이력 연계 → RFM·ABC 분석으로 기존 2등급 → 6등급 세분화, 카이제곱 검정 p &lt; 0.05 통계적 유의성 확보</p>
<p class="project-impact">정량 기반 등급 기준 수립 및 자동 최신화 파이프라인 구축, 영업 우선순위 재편 근거 마련</p>
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

<div class="project-card" id="project-jobsonar">
<h3>JobSonar - 데이터직군 채용공고 수집 및 조회 서비스<span class="badge-live">업데이트 중</span></h3>
<p class="project-problem"><strong>문제:</strong> 데이터직군 채용 트렌드를 파악하려면 여러 플랫폼을 수동으로 순회해야 함</p>
<p class="project-result"><strong>결과:</strong> 크롤러로 원티드·사람인·잡코리아 공고 수집 → jobs·job_skills 정규화 스키마 설계(외래키·UNIQUE 제약·인덱스) → SQL 집계 쿼리 기반 스택 트렌드·연봉 분포·공동 출현 네트워크 분석 → Dash 대시보드 배포</p>
<p class="project-impact">크롤링 → DB 설계 → SQL 집계 → 시각화까지 데이터 파이프라인 전 과정을 직접 설계·구현</p>
<div class="project-tags">
  <span class="tag">Python</span>
  <span class="tag">SQL</span>
  <span class="tag">SQLite</span>
  <span class="tag">Web Crawling</span>
  <span class="tag">Dash</span>
</div>
<div class="project-links">
  <a class="project-link" href="https://github.com/icedo724/JobSonar"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path></svg> GitHub</a>
  <a class="project-link" href="https://huggingface.co/spaces/mininiming/jobsonar"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="18" y1="20" x2="18" y2="10"></line><line x1="12" y1="20" x2="12" y2="4"></line><line x1="6" y1="20" x2="6" y2="14"></line></svg> 대시보드</a>
</div>
</div>

<div class="project-card">
<h3>리그오브레전드 상위 플레이어 메타 대시보드 구축</h3>
<p class="project-problem"><strong>배경:</strong> Riot API로 실제 데이터를 직접 수집하고, 메타 통계 사이트와 유사한 분석 대시보드를 처음부터 구현해보는 것이 목표</p>
<p class="project-result"><strong>결과:</strong> 마스터 이상 매치 데이터 수집 → 챔피언별 픽률-승률 사분면 분류(OP·숨겨진 강자·인기챔·비추) + 아이템 트리 상관관계 통계 검정 + 대시보드 배포</p>
<p class="project-impact">API 수집 → 통계 분석 → 시각화 → 배포까지 전 과정을 직접 구현하며 데이터 파이프라인 흐름 체득</p>
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

<div class="project-card" id="project-loaquant">
<h3>로스트아크 경제 시계열 분석<span class="badge-live">업데이트 중</span></h3>
<p class="project-problem"><strong>문제:</strong> 재화 가격이 왜 오르내리는지 원인 불명확 — 패키지·방송·업데이트 등 이벤트가 실제로 얼마나 충격을 주는지 정량화 수단 없음</p>
<p class="project-result"><strong>결과:</strong> 공식 API로 재화 시계열 수집 → ARIMA·Prophet 이원 적용, MAPE 1.29~5.19% 달성, 비정기 이벤트 충격 최대 ±14% 정량화, 재화 유형별 수요일 효과 반전 패턴 발견</p>
<p class="project-impact">정기적 효과·이벤트 레이어를 탑재한 1시간 단위 업데이트 대시보드로 "구매 적기" 판단 근거 제공</p>
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
<p class="project-problem"><strong>문제:</strong> 고레벨 구간에서 경험치 효율에 실제로 영향을 주는 요인이 무엇인지 정량적으로 밝혀진 바 없음 — 커뮤니티 경험담에만 의존</p>
<p class="project-result"><strong>결과:</strong> Nexon API로 Lv.285+ 유저 96,000명+ 경험치 데이터 수집 → 쇼케이스 전후 대응표본 t-검정(p &lt; 0.001), Lv.290~294 구간 +98.3% 증가 확인, 썬데이메이플 유형별 ANOVA(F=7,099, p &lt; 0.001)로 이벤트 효과 검증</p>
<p class="project-impact">96,000명 실데이터로 쇼케이스·이벤트가 레벨별 사냥 행동에 미치는 영향을 통계적으로 입증 — 커뮤니티 경험담을 수치로 검증</p>
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
<h3>LOABAL - 로스트아크 커뮤니티 감정분석</h3>
<p class="project-problem"><strong>문제:</strong> 패치 전후 유저 여론 변화를 정량화할 수단 없음 — 게임사 입장에서 수천 개 게시글을 읽지 않고 여론 방향을 파악해야 하는 상황</p>
<p class="project-result"><strong>결과:</strong> 로스트아크 인벤 직업 게시판 크롤링 → 2,929건 전량 직접 라벨링(4클래스) → KoBERT 기반 감정 분류 모델 v5 학습 완료 (범용 Macro F1 0.63, 딜러 Macro F1 0.63)</p>
<p class="project-impact">패치 전후 유저 감성 점수 시계열 시각화 → "이번 패치에 유저들이 어떻게 반응했는가"를 정량으로 제시 가능</p>
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
<h3>월드 오브 워크래프트 한밤 경제 분석<span class="badge-live">업데이트 중</span></h3>
<p class="project-problem"><strong>문제:</strong> 로스트아크 분석 경험을 다른 게임 경제에도 적용할 수 있는지 확인하고 싶었음 — WoW는 사전 도메인 지식이 전혀 없는 환경</p>
<p class="project-result"><strong>결과:</strong> Blizzard API로 30일+ 경매장 시세·등록량 1시간 단위 수집 → 한밤 출시 시 구재료 최대 -83% / 신재료 최대 +827% 전환 충격 정량화, WoW 토큰 시세 최고가(301,991G) 대비 시즌1 이후 -29.8% 하락 추적</p>
<p class="project-impact">도메인 지식 없이 데이터 패턴만으로 경제 구조 해석에 성공 — 로스트아크 분석 프레임워크의 이식 가능성 확인</p>
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
<p class="project-problem"><strong>문제:</strong> 패치마다 챔피언 너프·버프 방향을 예측하는 정량 기준 없음 — 유저와 분석가 모두 패치 노트 공개 전까지 추측에 의존</p>
<p class="project-result"><strong>결과:</strong> (진행 중) 마스터 이상 매치 로그 수집 (패치 16.1~16.6, 약 3개월치) → 포지션·승률·픽률·밴률 기반 분류·회귀 모델 v5 학습 완료</p>
<p class="project-impact"><strong>목표:</strong> 1년치 데이터(약 24패치) 수집 완료 후 패치 방향 예측 정확도 검증 및 배포</p>
<div class="project-progress">
  <span class="progress-label">진행률 약 25%</span>
  <div class="progress-bar"><div class="progress-fill" style="width: 25%"></div></div>
  <span class="progress-note">현재: 6패치분 수집 완료 · 목표 24패치 (1년치)</span>
</div>
<div class="project-tags">
  <span class="tag">Python</span>
  <span class="tag">Riot API</span>
  <span class="tag">회귀 모델</span>
  <span class="tag">분류 모델</span>
</div>
<div class="project-links">
  <a class="project-link" href="https://github.com/icedo724/Loracle"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path></svg> GitHub</a>
</div>
</div>

## 공모전 및 기타 저장소

<div class="project-card">
<h3>제6회 교육 공공데이터 분석·활용대회<span class="badge-entry">참가</span></h3>
<p class="project-problem"><strong>문제:</strong> 서울시 특수유아 분포와 특수교사 배치 현황 간 불균등 의심 — 데이터 기반 검증 없이 정책 입안 중</p>
<p class="project-result"><strong>결과:</strong> 공공데이터 다중 연계 + 다중 회귀 모델링으로 배치 불균등 통계적 검증, 지역별 우선 배치 필요 구간 식별</p>
<p class="project-impact">데이터 기반 특수교사 배치 우선 지역 도출 및 정책적 개선안 제시</p>
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
<h3>제6회 서울교육 데이터 분석·활용 공모전<span class="badge-entry">참가</span></h3>
<p class="project-problem"><strong>문제:</strong> 특수교육 대상자와 교육 기관의 공간적 불일치 — 어디에 신규 특수학교를 지어야 하는지 데이터 근거 부재</p>
<p class="project-result"><strong>결과:</strong> 대상자 분포 + 기관 접근성 지수 공간 분석 → 수요 대비 공급 부족 지역 정량화, 최적 설립 후보지 도출</p>
<p class="project-impact">데이터 기반 신규 특수학교 설립 우선 지역 제안 — 예산 투입 효율 최대화 방안</p>
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
