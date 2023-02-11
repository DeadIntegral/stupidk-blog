---
title: dev-weekly 2022-10-15
date: "2022-10-15T22:00:00.000Z"
description: "dev-weekly 2022-10-15"
tags: ["javascript", "css", "node"]
---
# CSS

### **[Layout Breakouts with CSS Grid](https://ryanmulligan.dev/blog/layout-breakouts)**

- grid-template-columns 에 명명된 그리드를 활용한 레이아웃 브레이크

### **[Making a Real-Time Clock With a Conic Gradient Face](https://css-tricks.com/making-a-real-time-clock-with-a-conic-gradient-face)**

- 원뿔 그라디언트로 시계 만들기
- `.style.setProperty("--second-hand-degrees", secondsAngle + "deg");` 를 통한 css variable 제어

# Node

### **[Knip: Find Unused Files, Dependencies and Exports in TypeScript Projects](https://github.com/webpro/knip)**

- JS/TS 프로젝트에서 사용하지 않는 파일, 의존성을 추출하는 도구
- [https://github.com/webpro/knip#comparison](https://github.com/webpro/knip#comparison)

### **[human-signals: Human-Friendly Process Signal Info](https://github.com/ehmicky/human-signals)**

- POSIX 시그널을 사람 친화적으로 표현해주는 도구
- [https://github.com/ehmicky/human-signals/blob/main/src/core.js](https://github.com/ehmicky/human-signals/blob/main/src/core.js)

# Javascript

### **[Intl Explorer: A Way to Learn and Experiment with the ECMAScript Internationalization API](https://www.intl-explorer.com/?locale=ko)**

- Intl 를 실험하고 사용해보는 도구 및 플레이그라운드

### **[Node v18.11.0 (Current) Released; Gains 'Watch Mode'](https://nodejs.org/en/blog/release/v18.11.0/)**

- watch 기능 실험적 제공. nodemon처럼 파일이 변경되면 프로세스 다시 시작.

### **[Lerna Reborn: What’s New in Version 6?](https://blog.nrwl.io/lerna-reborn-whats-new-in-v6-10aec6e9091c)**

- 캐싱을 디폴트로 변경(useNx), 원격 캐싱 지원(Nx Cloud)
- PNPM 지원
- workspace를 위한 VSCode 익스텐션

### **[First-class Vite support in Storybook](https://storybook.js.org/blog/first-class-vite-support-in-storybook/)**

- 성능을 위해 pre-bundled 로 제공하고, webpack을 vite로 변경
- zero config 지원
- 다양한 생태계 지원(React, Vue2,3, Svelte, SvelteKit. Lit 등) - 추가 구성 없이 작동

### **[State of GraphQL](https://2022.stateofgraphql.com/ko-KR/)**

- State of GraphQL 첫 설문조사 결과

### **[Choosing the Best Node.js Docker Image](https://snyk.io/blog/choosing-the-best-node-js-docker-image/)**

- nodejs docker 이미지 비교
    - 버전, 종속성, 각 취약점, 런타임 취약점, 이미지 크기 등

### **[Why We Use Babylon.js Instead of Three.js in 2022](https://www.spotvirtual.com/blog/why-we-use-babylonjs-instead-of-threejs-in-2022)**

- Threejs와 바빌론 비교 - TS지원, 아키텍쳐, 툴링 등
    - 서로 목적이 다름
- 커뮤니티 지원 - 모든 버그는 24시간 내 수정
- react three fiber 등 리액트 연동

### **[How to Build SVG Line Charts with React, SSR and Tailwind CSS](https://thenewstack.io/how-to-build-svg-line-charts-with-react-ssr-and-tailwind-css/)**

- 갯츠비 및 넥스트js에서 SVG 라인 차트 만들기 (tailwind로 스타일링)

### **[Javet 2.0.0: Embed Node and V8 in Java Apps](https://www.caoccao.com/Javet/)**

- Java에 nodejs와 v8을 임베딩하는 도구

### **[Sortable: Create and Reorder Lists with Drag-and-Drop](http://sortablejs.github.io/Sortable/)**

- 모던 브라우저 및 터치 장치를 지원
- 오토 스크롤, CSS Animation, 멀티 드래그 지원 등

### **[melonJS 14.0: A Lightweight 2D Game Engine](https://github.com/melonjs/melonJS/releases)**

- core, test unit 등에서 ES5 deprecate