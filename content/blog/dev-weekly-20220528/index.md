---
title: dev-weekly 2022-05-28
date: "2022-05-28T11:00:00.000Z"
description: "dev-weekly 2022-05-28"
tags: ["javascript", "css", "node"]
---

# CSS

### **[Lesser-Known And Underused CSS Features In 2022](https://www.smashingmagazine.com/2022/05/lesser-known-underused-css-features-2022/)**

- 잘 알려지지 않은 CSS 속성과 셀렉터에 대한 설명
- `All`, `currentColor`, fallback, interaction media query, `scroll-padding`, ****`font-variant`, `isolation`, `content-visibility`…
- Counter(`counter-reset`, `reversed`, `counter-increment`, `counter`)

### **[Building a Button Component](https://web.dev/building-a-button-component)**

- 접근성, 스타일을 고려한 버튼 만들기

### **[A Perfect Table of Contents With HTML + CSS](https://css-tricks.com/a-perfect-table-of-contents-with-html-css)**

- html, css로 목차 만들기
- 올바른 마크업, 스타일링(CSS로 그려는 점선), 접근성(점선을 읽지 않도록)

# Node

### **[TypeScript 4.7 Released](https://devblogs.microsoft.com/typescript/announcing-typescript-4-7/)**

- TS 4.7 릴리즈
- package.json - type의 새로운 확장, 새 파일 확장자
- 모듈 감지 제어 - 기존 스크립트 코드와 새 모듈 코드
- Go to Source Definition - .d.ts 파일에 가려져 있더라도 원본 코드를 찾아가는 기능

### **[run GitHub Actions in a Node 16 runtime](https://github.blog/changelog/2022-05-20-actions-can-now-run-in-a-node-js-16-runtime/)**

- 깃헙액션에서 노드16 지원

### **[Electron 19.0.0 Released](https://www.electronjs.org/blog/electron-19-0)**

- 크롬102, V8 10.2, Node 16.14.2 포함

# Javascript

### **[Next.js's Layouts RFC: Big Changes Ahead for Next.js](https://nextjs.org/blog/layouts-rfc)**

- layout.js - 하위 트리의 라우트 세그먼트 간에 공유되는 UI
- page.js - 라우트 세그먼트에 고유하고, 유효하기 위해 필요한 UI
- 리액트 서버 컴포넌트

### [Angular 14 (currently in RC phase)](https://nevzatopcu.medium.com/what-is-new-in-angular-14-d31edf91fd3e)

- 앵귤러 14 기능 소개

### **[How Airbnb Gets Faster JavaScript Builds with Metro](https://medium.com/airbnb-engineering/faster-javascript-builds-with-metro-cfc46d617a1f)**

- 에어비앤비의 Metro 변경 후 개선점
- Metro 와 Webpack의 아키텍처 차이

### **[The Balance Has Shifted Away From SPAs](https://nolanlawson.com/2022/05/21/the-balance-has-shifted-away-from-spas/)**

- 최근 SPA보다 MPA에 생겨난 장점들
    - Paint Holding - same origin에는 flush of white 감소
    - bfcache - 페이지의 전체 스냅샷을 저장하는 메모리 내 캐시
    - Service worker - 클라이언트 라우터 대신 오프라인 탐색
    - Shared Element Transitions - MPA 페이지 전환 간 애니메이션

### **[Ninja Keys: Add a Command Palette / Keyboard Shortcuts Interface to Your App/Site](https://github.com/ssleptsov/ninja-keys)**

- 바닐라, 리액트, 뷰, 스벨트를 지원하는 커맨드 팔레트 + 키보드 단축키 인터페이스
- [https://github.com/timc1/kbar](https://github.com/timc1/kbar)

### **[EStimator.dev: The Modern JavaScript Savings Calculator](https://estimator.dev/)**

- 사이트를 입력 시 사이트의 각 js파일을 최신 문법으로 변경했을 때 크기. 성능, 영향 계산
- [https://github.com/GoogleChromeLabs/estimator.dev](https://github.com/GoogleChromeLabs/estimator.dev)