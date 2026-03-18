---
layout: home
title: Home
---

# 안녕하세요, 데이터 분석가 조민서입니다.

우연한 계기로 데이터의 매력에 빠져, 이제는 데이터 속에서 길을 찾는 분석가로 성장하고 있습니다.<br>
축적된 데이터를 다각도로 분석하여 전체적인 흐름과 트렌드를 읽어내는 작업을 즐깁니다.<br>
단순한 수치를 넘어, 탄탄한 논리적 근거를 바탕으로 데이터 이면에 숨겨진 스토리를 풀어내고자 합니다.

<script>
  // 페이지가 나타나고 0.2초 뒤에 아이콘을 싹 바꿔치기하는 마법의 코드입니다.
  setTimeout(function() {
    var cvIcon = document.querySelector('a[href*="/cv"]');
    var projIcon = document.querySelector('a[href="/projects/"]');

    if (cvIcon && projIcon) {
      // 1. 스택오버플로우 모양을 -> 프로젝트 느낌의 '코드(</>)' 아이콘으로 변경
      projIcon.innerHTML = '<svg width="24" height="24" stroke-width="1.5" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" color="currentColor"><path d="M13.5 6L10 18.5" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"></path><path d="M6.5 8.5L3 12L6.5 15.5" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"></path><path d="M17.5 8.5L21 12L17.5 15.5" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"></path></svg>';
      
      // 2. 맨 왼쪽에 있던 아이콘을 -> CV 아이콘의 바로 오른쪽으로 이동
      cvIcon.parentNode.insertBefore(projIcon, cvIcon.nextSibling);
    }
  }, 200);
</script>