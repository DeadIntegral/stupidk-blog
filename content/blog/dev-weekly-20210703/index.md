---
title: dev-weekly 2021-07-03
date: "2021-07-03T09:30:00.000Z"
description: "dev-weekly 2021-07-03"
tags: ["javascript", "node", "css"]
---

## Node

### [GitHub Copilot: An AI 'Pair Programmer'](https://copilot.github.com/)

- github이 openAI 로 개발한 ai 추천 스니펫

### [Encoding Data for POST Requests Properly](https://jakearchibald.com/2021/encoding-data-for-post-requests/)

- Copilot의 예제가 보안에 좋지 않다고 개선하는 아티클
- URLSearchParams 와 FormData 을 사용한 올바른 HTTP body 설명

### [Piscina: A Fast Worker Thread Pool Implementation](https://github.com/piscinajs/piscina)

- 노드 워커 스레드 풀 구현

## CSS

### [A 3D Hover Effect Using CSS Transforms](https://letsbuildui.dev/articles/a-3d-hover-effect-using-css-transforms)

- 3d hover effect - mouse방향으로 기울어지는 효과
- 기본적으로 transform과 will-change를 사용하나 커서 위치와 관련된 영역에서 js 이용
- 웹 접근성에 대한 고려 및, 글 중간중간 왜 이렇게 구현하는지에 대한 설명이 있는 글

### [Positioning Overlay Content with CSS Grid](https://css-tricks.com/positioning-overlay-content-with-css-grid)

- grid로 position overlay 하기
- 캐러셀에 텍스트 버튼 등 배치하기

# Javascript

### [Solid 1.0: A Declarative JavaScript UI Library Worth Investigating](https://dev.to/ryansolid/solidjs-official-release-the-long-road-to-1-0-4ldd)

- 리액트의 유연성과 스벨트의 심플한 멘탈 모델을 갖춘 라이브러리
- vdom 대신 reactive + precompiled
- redux, Xstate 호환
- Concurrent Rendering 지원 계획 및 vite를 사용한 Isomorphic Starter 지원 계획

### ['next generation' of rendering engine for Chrome](https://developer.chrome.com/blog/renderingng/)

- 크롬의 차세대 렌더링 엔진 RendererNG
- CompositAfterPaint, LayoutNG, BlinkNG, GPU Acceleration everywhere, Threaded scrolling, animations, and decode, Viz, Threaded and accelerated canvas rendering, VideoNG 프로젝트
- 웹과 크롬에서 더이상 렌더링 속도 향상에 대한 기대가 어렵기 때문에, 새로운 기반 구축

### [Google has delayed its plans to block third-party cookies](https://www.theverge.com/2021/6/24/22547339/google-chrome-cookiepocalypse-delayed-2023)

- 크롬의 써드 파티 쿠키 차단은 2023년까지 연기

### [Sorting Colors in JavaScript](https://tomekdev.com/posts/sorting-colors-in-js)

- JS로 색상 정렬하기
- hex와 rgba, alpha로 인한 영향(블렌딩), 비슷한 색상끼리의 카테고라이징(벡터 계산)

## Code & Tools

### [Google's New Tool for Understanding Package Dependencies](https://deps.dev/)

- [https://deps.dev/](https://deps.dev/) - npm, go, maven, cargo까지 지원

### [Million: A Less-than-1KB Virtual DOM Implementation](https://million.js.org/)

- 기존의 가상돔은 너무 복잡하고 무거워서 만들었다는 가상돔
- library-agnostic 한 가상돔을 만드는 것이 목적
- [https://github.com/aidenybai/million](https://github.com/aidenybai/million)

### [A Fortnite-Inspired VS Code Theme](https://marketplace.visualstudio.com/items?itemName=sdras.fortnite-vscode-theme#fortnitetheme)

- VSCode 포트나이트 테마