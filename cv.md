---
layout: cv
title: CV
---
<style>
  @import url('https://cdn.jsdelivr.net/gh/orioncactus/pretendard/dist/web/static/pretendard.css');
  body, h1, h2, h3, h4, h5, h6, p, li, a {
    font-family: 'Pretendard', -apple-system, BlinkMacSystemFont, system-ui, Roboto, 'Helvetica Neue', 'Segoe UI', 'Apple SD Gothic Neo', 'Noto Sans KR', sans-serif !important;
  }
  .skill-group {
    display: flex;
    align-items: baseline;
    gap: 10px;
    margin-bottom: 0.5em;
    flex-wrap: wrap;
  }
  .skill-label {
    font-size: 0.8em;
    font-weight: 600;
    color: var(--color-text);
    opacity: 0.6;
    min-width: 5em;
    flex-shrink: 0;
  }
  .skill-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 6px;
  }
  .skill-tag {
    background-color: var(--color-border);
    color: var(--color-text);
    padding: 2px 10px;
    border-radius: 12px;
    font-size: 0.78em;
    font-weight: 500;
  }
  .game-platform {
    margin-bottom: 0.9em;
  }
  .game-platform-label {
    font-size: 0.78em;
    font-weight: 700;
    opacity: 0.5;
    text-transform: uppercase;
    letter-spacing: 0.05em;
    margin-bottom: 0.35em;
  }
  .game-entry {
    display: grid;
    grid-template-columns: 11em 8em 1fr;
    font-size: 0.85em;
    padding: 1px 0;
  }
  .game-name {
    font-weight: 600;
  }
  .game-genre {
    opacity: 0.6;
  }
  .game-period {
    opacity: 0.5;
    font-size: 0.92em;
  }
  .game-more-toggle {
    margin-top: 0.6em;
    margin-bottom: 0.4em;
  }
  .game-more-toggle > summary {
    list-style: none;
    cursor: pointer;
    display: inline-flex;
    align-items: center;
    gap: 6px;
    font-size: 0.8em;
    opacity: 0.55;
    user-select: none;
    padding: 2px 0;
  }
  .game-more-toggle > summary::-webkit-details-marker { display: none; }
  .game-more-toggle > summary::before {
    content: '▶';
    font-size: 0.7em;
    transition: transform 0.2s;
  }
  .game-more-toggle[open] > summary::before {
    transform: rotate(90deg);
  }
  .game-more-toggle > summary:hover { opacity: 0.85; }
  .series-toggle {
    margin: 0.6em 0 0.2em 0;
  }
  .series-toggle > summary {
    list-style: none;
    cursor: pointer;
    display: inline-flex;
    align-items: center;
    gap: 6px;
    font-size: 0.82em;
    font-weight: 600;
    user-select: none;
    padding: 2px 0;
  }
  .series-toggle > summary::-webkit-details-marker { display: none; }
  .series-toggle > summary::before {
    content: '▶';
    font-size: 0.65em;
    opacity: 0.5;
    transition: transform 0.2s;
  }
  .series-toggle[open] > summary::before {
    transform: rotate(90deg);
  }
  .series-toggle > summary:hover { opacity: 0.75; }
  .series-list {
    list-style: none;
    padding: 0.3em 0 0.3em 1.2em;
    margin: 0;
  }
  .series-list li {
    font-size: 0.82em;
    opacity: 0.75;
    padding: 1px 0;
    line-height: 1.6;
  }
</style>

# 학력 및 자격

## 학력
* **한국방송통신대학교** | 통계·데이터과학과 (2024.09 ~ 재학 중)
* **숭실대학교 전산원** | 컴퓨터공학과 (2019.03 ~ 2023.08)

## 교육
* **프로그래머스 데이터 분석 데브코스** | 부트캠프 수료 (2023.11 ~ 2024.04)

## 자격
* **국가공인 SQL개발자(SQLD)** | 한국데이터산업진흥원 (2026.03)
* **빅데이터분석기사** | 한국데이터산업진흥원 (2025.12)
* **정보처리산업기사** | 한국산업인력공단 (2021.08)
* **네트워크관리사 2급** | 한국정보통신자격협회 (2020.01)

## 기술

<div class="skill-group">
  <span class="skill-label">언어</span>
  <div class="skill-tags">
    <a class="skill-tag" href="/projects/#project-loaquant" style="text-decoration:none; color:inherit;">Python</a>
    <span class="skill-tag">R</span>
    <a class="skill-tag" href="/projects/#project-jobsonar" style="text-decoration:none; color:inherit;">SQL</a>
  </div>
</div>
<div class="skill-group">
  <span class="skill-label">도구</span>
  <div class="skill-tags">
    <span class="skill-tag">Power BI</span>
    <span class="skill-tag">Tableau</span>
  </div>
</div>

## 게임
<div class="game-platform">
  <div class="game-platform-label">PC</div>
  <div class="game-entry">
    <span class="game-name">메이플스토리</span>
    <span class="game-genre">MMORPG</span>
    <span class="game-period">10년 이상</span>
  </div>
  <div class="game-entry">
    <span class="game-name">로스트아크</span>
    <span class="game-genre">MMORPG</span>
    <span class="game-period">1년 이상</span>
  </div>
  <div class="game-entry">
    <span class="game-name">리그오브레전드</span>
    <span class="game-genre">MOBA</span>
    <span class="game-period">10년 이상</span>
  </div>
  <div class="game-entry">
    <span class="game-name">전략적 팀 전투</span>
    <span class="game-genre">오토배틀러</span>
    <span class="game-period">5년 이상</span>
  </div>
</div>

<div class="game-platform">
  <div class="game-platform-label">Mobile</div>
  <div class="game-entry">
    <span class="game-name">마비노기 모바일</span>
    <span class="game-genre">MMORPG</span>
    <span class="game-period">1년 이상</span>
  </div>
  <div class="game-entry">
    <span class="game-name">AFK 새로운 여정</span>
    <span class="game-genre">방치형 RPG</span>
    <span class="game-period">1년 이상</span>
  </div>
</div>

<div class="game-platform">
  <div class="game-platform-label">Console</div>
  <div class="game-entry">
    <span class="game-name">포켓몬스터 시리즈</span>
    <span class="game-genre">RPG</span>
    <span class="game-period">10년 이상</span>
  </div>
  <div class="game-entry">
    <span class="game-name">몬스터헌터 시리즈</span>
    <span class="game-genre">RPG</span>
    <span class="game-period">2년 이상</span>
  </div>
  <div class="game-entry">
    <span class="game-name">슈퍼마리오 시리즈</span>
    <span class="game-genre">플랫폼 게임</span>
    <span class="game-period">10년 이상</span>
  </div>
  <details class="game-more-toggle">
    <summary>플레이한 게임 타이틀 전체보기</summary>
    <p style="font-size:0.78em; opacity:0.5; margin: 0.3em 0 0.6em 0;">엔딩 크레딧 확인 기준</p>
    <details class="series-toggle">
      <summary>포켓몬스터 시리즈</summary>
      <ul class="series-list">
        <li>본가 2~9세대 메인 시리즈</li>
        <li>Pokémon LEGENDS 아르세우스</li>
        <li>Pokémon LEGENDS Z-A</li>
        <li>포켓몬 포코피아</li>
        <li>포켓몬 챔피언스</li>
      </ul>
    </details>
    <details class="series-toggle">
      <summary>젤다의 전설 시리즈</summary>
      <ul class="series-list">
        <li>몽환의 모래시계</li>
        <li>스카이워드 소드</li>
        <li>브레스 오브 더 와일드</li>
        <li>티어스 오브 더 킹덤</li>
        <li>지혜의 투영</li>
      </ul>
    </details>
    <details class="series-toggle">
      <summary>슈퍼마리오 시리즈</summary>
      <ul class="series-list">
        <li>뉴 슈퍼 마리오브라더스</li>
        <li>마리오 파티 DS</li>
        <li>뉴 슈퍼 마리오브라더스 Wii</li>
        <li>마리오 카트 Wii</li>
        <li>슈퍼 마리오 갤럭시 1·2</li>
        <li>슈퍼 마리오 64</li>
        <li>슈퍼 마리오 메이커 2</li>
        <li>슈퍼 마리오 오디세이</li>
        <li>마리오 카트 월드</li>
        <li>동키콩 바난자</li>
      </ul>
    </details>
    <details class="series-toggle">
      <summary>몬스터헌터 시리즈</summary>
      <ul class="series-list">
        <li>몬스터 헌터 월드·아이스본</li>
        <li>몬스터 헌터 라이즈·선브레이크</li>
        <li>몬스터 헌터 와일즈</li>
      </ul>
    </details>
    <details class="series-toggle">
      <summary>이외 콘솔게임</summary>
      <ul class="series-list">
        <li>다크 소울 1·2·3</li>
        <li>엘든 링</li>
        <li>세키로: 섀도우 다이 트와이스</li>
        <li>클레르 옵스퀴르: 33 원정대</li>
        <li>붉은사막 (플레이 진행중)</li>
      </ul>
    </details>
  </details>
</div>

<div style="text-align: center; margin-bottom: 40px; margin-top: 20px;">
  <p style="margin-top: 15px; font-size: 0.7em; display: flex; justify-content: center; align-items: center; gap: 7px; flex-wrap: wrap; opacity: 0.8;">

    <span style="display: flex; align-items: center; gap: 4px;">
      <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path><polyline points="22,6 12,13 2,6"></polyline></svg>
      <a href="mailto:{{ site.author.email }}" style="color: inherit; text-decoration: none;">{{ site.author.email }}</a>
    </span>

    <span style="opacity: 0.3; margin: 0 2px;">|</span>

    <span style="display: flex; align-items: center; gap: 4px;">
      <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"></path></svg>
      {{ site.phone }}
    </span>

    <span style="opacity: 0.3; margin: 0 2px;">|</span>

    <span style="display: flex; align-items: center; gap: 4px;">
      <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"></path><circle cx="12" cy="10" r="3"></circle></svg>
      {{ site.address }}
    </span>

  </p>
</div>
<hr style="border: 0; border-top: 1px solid currentColor; opacity: 0.15; margin-bottom: 40px;">