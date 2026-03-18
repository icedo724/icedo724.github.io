---
layout: home
title: Home
---

# About

# 안녕하세요, 데이터 분석가 조민서입니다.

우연한 계기로 데이터의 매력에 빠져, 이제는 데이터 속에서 길을 찾는 분석가로 성장하고 있습니다.
축적된 데이터를 다각도로 분석하여 전체적인 흐름과 트렌드를 읽어내는 작업을 즐깁니다.
단순한 수치를 넘어, 탄탄한 논리적 근거를 바탕으로 데이터 이면에 숨겨진 비즈니스 스토리를 명쾌하게 풀어내고자 합니다.

<script>
document.addEventListener("DOMContentLoaded", function() {
    // 1. 화면에서 기존 CV 아이콘 찾기
    const cvLink = document.querySelector('a[href*="/cv"]');
    
    if (cvLink) {
        // 2. 프로젝트 링크 뼈대 만들기
        const projLink = document.createElement('a');
        projLink.href = '/projects/';
        projLink.title = 'Projects';
        projLink.className = cvLink.className; // CV 아이콘과 완전히 동일한 테마 디자인 적용
        
        // 3. 프로젝트 느낌이 나는 '코드(Code)' 모양의 SVG 아이콘 삽입
        projLink.innerHTML = `<svg width="24px" height="24px" stroke-width="1.5" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" color="currentColor"><path d="M13.5 6L10 18.5" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"></path><path d="M6.5 8.5L3 12L6.5 15.5" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"></path><path d="M17.5 8.5L21 12L17.5 15.5" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"></path></svg>`;
        
        // 4. CV 아이콘 바로 옆(뒤)에 딱 붙여서 삽입
        cvLink.parentNode.insertBefore(projLink, cvLink.nextSibling);
    }
});
</script>