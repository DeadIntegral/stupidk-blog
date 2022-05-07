---
title: dev-weekly 2022-05-07
date: "2022-05-07T23:45:00.000Z"
description: "dev-weekly 2022-05-07"
tags: ["javascript", "css", "node"]
---

# CSS

### **[Contextual Spacing For Intrinsic Web Design](https://moderncss.dev/contextual-spacing-for-intrinsic-web-design)**

- 뷰포트 기준 미디어 쿼리는 모든 컨텍스트에 확장할 수 없음
- 본질적인 디자인을 위한 프로퍼티, 함수 소개 - clamp(), fit-content, grid 등
- padding은 clamp()로, margin은 block start로, gap은 clamp()로 사용하여 제어 할 때의 장점

### **[Deep Dive into Text Wrapping and Word Breaking](https://codersblock.com/blog/deep-dive-into-text-wrapping-and-word-breaking)**

- overflow-wrap(과거의 word-wrap), word-break 등의 CSS 제어
- `<wbr>`, `shy;`, `&nbsp;`**,** `&NoBreak;` 등을 이용한 제어
- CJK(한중일)에서 동작시키기 위한 CSS Property

### **[Flexibly Centering an Element with Side-Aligned Content](https://meyerweb.com/eric/thoughts/2022/04/26/flexibly-centering-an-element-with-side-aligned-content)**

- 텍스트는 좌측 정렬을 유지하면서 영역은 가운데 정렬하기
- wrapper를 만드는 고전적인 방법, wrapper가 없어도 되는 요즘 방법

### **[CSS-Only Pokémon Quest Icon Sorter](https://codepen.io/gabriellewee/pen/KKQwydY)**

- html, css로 만든 포켓몬 퀘스트의 아이콘들

# Node

### **[Node v18.1.0 (Current) Released](https://nodejs.org/en/blog/release/v18.1.0/)**

- Node 18.1.0 릴리즈
- https://github.com/nodejs/node/pull/42701 - WASM Web API에 대한 추가 개발

### **[The Thing About Fastify](https://hire.jonasgalvez.com.br/2022/may/02/the-thing-about-fastify/)**

- fastify에 대하여 - 장점들
- Hooks, 요청과 응답확장, 플러그인 캡슐화, 워커 지원 등

### **[Creating and Deploying a Tiny Proxy Server on Vercel in 10 Minutes](https://mmazzarolo.com/blog/2022-02-05-creating-and-deploying-a-proxy-server-in-5-minutes/)**

- vercel과 http-proxy-middleware를 사용하여 10분만에 프록시 서버 만들기

### **[resvg-js 2.0: A High-Performance SVG Renderer and Toolkit](https://github.com/yisibl/resvg-js)**

- 러스트 기반의 resvg, napi-rs. `.node` 로 컴파일되어 node-gyp가 필요하지 않음
- 제로 디펜던시, SVG to PNG, SVG텍스트에서 시스템 폰트, 사용자 폰트 지원

# Javascript

### **[How Partytown Eliminates Website Bloat From Third-Party Scripts](https://www.smashingmagazine.com/2022/04/partytown-eliminates-website-bloat-third-party-apps/)**

- Partytown 라이브러리에 대한 소개
- 파티타운의 아키텍쳐와 작동원리
- 파티타운 사용법(설정)

### **[Ryan Dahl on 'JavaScript Containers'](https://tinyclouds.org/javascript_containers)**

- 

### **[Babylon.js 5.0: The Powerful 3D Rendering Engine](https://babylonjs.medium.com/babylon-js-5-0-beyond-the-stars-2d11d4c3d07)**

- 바빌론 5.0 릴리즈 -

### RELEASES

- pnpm 7.0
    - [https://github.com/pnpm/pnpm/releases/tag/v7.0.0](https://github.com/pnpm/pnpm/releases/tag/v7.0.0)
- Mocha 10.0
    - [https://github.com/mochajs/mocha/releases/tag/v10.0.0](https://github.com/mochajs/mocha/releases/tag/v10.0.0)

### **[Porting Zelda Classic to the Web](https://hoten.cc/blog/porting-zelda-classic-to-the-web/)**

- a

### **[React Toastify 9.0: Notification Boxes Made Easy in React Apps](https://github.com/fkhadra/react-toastify/releases/tag/v9.0.0)**

- React Toastify 9.0 릴리즈 - 에드온 추가
- useNotificationCenter 헤드리스 훅, StackedContainer
- toast.onChange변경, toast.confiure 제거