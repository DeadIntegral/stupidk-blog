---
title: dev-weekly 2022-04-30
date: "2022-04-30T09:50:00.000Z"
description: "dev-weekly 2022-04-30"
tags: ["javascript", "css", "node"]
---

# CSS

### **[Non-Interactive Elements With the Inert Attribute](https://webkit.org/blog/12578/non-interactive-elements-with-the-inert-attribute)**

- `disabled` 어트리뷰트는 form control 요소에서만 작동
- 과거 인터랙션 비활성화를 위한 테크닉들. `tabindex="-1"`, `user-select: none`
- 이들을 대신할 수 있는 `inert` 어트리뷰트 소개
- 지원: safari 15.5, chrome102, Firefox Nightly

### **[Linear-Style Cursor Glow](https://codepen.io/davidkpiano/pen/gOoNZNe)**

- 커서에 조명효과 입힌 데모

# Node

### **[Node 18's 'Prefix-Only' Core Modules](https://fusebit.io/blog/node-18-prefix-only-modules/)**

- 노드18에서 등장한 프리픽스 `node:` 의 등장 배경
- `node:test`는 node 프리픽스가 있어야만 가져올 수 있는 첫 핵심 모듈
- 장점: 노드 코어 모듈과 사용자 영역 모듈을 명확하게 구분 가능
- 단점: 모듈 시스템 불일치, 타이포스쿼팅 공격에 대한 가능성

### **[Node v16.15.0 (LTS) Released](https://nodejs.org/en/blog/release/v16.15.0/)**

- 노드18에도 fetch가 추가된것처럼, 16.15에도 fetch 추가(-experimental-fetch)

### **[Netlify Edge Functions: Serverless Compute Powered by Deno](https://www.netlify.com/blog/announcing-serverless-compute-with-edge-functions/)**

- 엣지 펑션 소개 및 quick start 가이드
- 지원하는 도구들 - Astro, nextjs, nuxt, remix, sveltekit 등
- 왜 deno로 구축했는지에 대한 netlify CEO의 설명
    - [https://thenewstack.io/netlify-ceo-on-why-netlify-edge-functions-was-built-on-deno](https://thenewstack.io/netlify-ceo-on-why-netlify-edge-functions-was-built-on-deno/)

### **[Knex.js 2.0: A Query Builder for Multiple Databases](https://github.com/knex/knex/releases/tag/2.0.0)**

- 쿼리 빌더 Knex 2.0 릴리즈

### **[Skia Canvas: A Canvas Environment for Node](https://github.com/samizdatco/skia-canvas)**

- 구글의 Skia 엔진을 기반으로 하는 Nodejs용 HTML canvas

# Javascript

### **[Building a JavaScript Bundler from Scratch](https://cpojer.net/posts/building-a-javascript-bundler)**

- JS 인프라 시리즈 4번째, 번들러 만들기
- 번들링에 필요한 과정(파일 시스템 검색, 종속성 그래프, 번들 직렬화, 병렬 컴파일)에 대한 설명 및 간단한 구축(다른 도구를 활용)

### **[Jest 28: JS Testing Gets Lighter, Faster, More Productive](https://jestjs.io/blog/2022/04/25/jest-28)**

- 샤딩, fake-timer, package.json export, 깃헙 액션 reporter 지원
    - Jest가 실행중인 global을 검사하고, 테스팅 환경에 누락된 global을 복사
- 마이그레이션 가이드 - [https://jestjs.io/docs/upgrading-to-jest28](https://jestjs.io/docs/upgrading-to-jest28)

### **[Figma Plugin for Storybook](https://storybook.js.org/blog/figma-plugin-for-storybook/)**

- 피그마와 스토리북 연결 - 시간의 흐름에 따라 source of truth 가 혼란스러워지는것을 극복하기위해
- 다양한 에드온들
    - Measure addon - 렌더링된 UI가 디자인과 일치하는지 검사해주는 도구. DOM Element와 디자인 스펙의 치수 비교
    - Outline addon - CSS 정렬 디버깅을 위해 각 DOM Element의 경계 시각화

### **Brief and Release**

- **[visual demo in just 256 bytes of JavaScript](https://twitter.com/KilledByAPixel/status/1517294627996545024)**
    - 256바이트로 만든 애니메이션 (고전)
- **[React 18.1](https://github.com/facebook/react/releases/tag/v18.1.0)**
    - 리액트 18.1 릴리즈

### **[Upgrading to React 18 with TypeScript](https://blog.logrocket.com/upgrading-react-18-typescript/)**

- `npx types-react-codemod preset-18 ./src` 를 사용하여 코드 자동 변경

### **[FortuneSheet: An Excel-Like JS Spreadsheet Control](https://github.com/ruilisi/fortune-sheet)**

- 액셀, 구글 스프레드 시트와 같은 JS 스프레드 시트 라이브러리
- [https://ruilisi.github.io/fortune-sheet-demo/?path=/story/workbook--basic](https://ruilisi.github.io/fortune-sheet-demo/?path=/story/workbook--basic)

### **[React Responsive Pagination: Component for Smart Pagination](https://github.com/jonelantha/react-responsive-pagination)**

- 반응형 페이지네이션 툴. 화면 크기에 비례한 페이지 숫자