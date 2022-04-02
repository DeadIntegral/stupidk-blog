---
title: dev-weekly 2022-04-02
date: "2022-04-02T14:00:00.000Z"
description: "dev-weekly 2022-04-02"
tags: ["javascript", "css", "node"]
---

# CSS

### **[Understanding Layout Algorithms](https://www.joshwcomeau.com/css/understanding-layout-algorithms)**

- CSS는 프로퍼티 모음이 아니라 상호 연결된 레이아웃 모드의 집합체
    - 요소를 렌더링하는데 사용할 레이아웃 모드를 파악하기
    - 가장 일반적인 레이아웃 Flow
        - flexbox에는 레이어 컨셉이 들어가있고, z-index를 사용 가능
    - ⇒ 레이아웃 모드에 따라 프로퍼티는 다르게 구현됨

### 참고

- [https://ageek.dev/css-layouts](https://ageek.dev/css-layouts)
- Default Layout(Flow Layout)
- Flexbox Layout
- Grid Layout
- Float Layout
- Positioned Layout
- Table Layout
- Multi-Column Layout

### **[A Guide To Hover And Pointer Media Queries](https://www.smashingmagazine.com/2022/03/guide-hover-pointer-media-queries)**

- hover, pointer 등의 media query
    - 포인터의 정확도 감지하기

### **[Optimising Largest Contentful Paint](https://csswizardry.com/2022/03/optimising-largest-contentful-paint)**

- LCP 개선 방안들 - 가급적 image없이, 이미지를 넣을 때 최적화 하는 방법들
- LCP는 lazy loading하는것 아님

### **[HTML Semantics](https://gomakethings.com/html-semantics)**

- 인터랙티브한 요소는 focus 가능하게 하기
- Button vs Link - [https://marcysutton.com/links-vs-buttons-in-modern-web-applications](https://marcysutton.com/links-vs-buttons-in-modern-web-applications)

### **[CSSUI](https://www.cssui.dev/)**

- 순수 HTML, CSS로 구현한 인터랙티브 컴포넌트 라이브러리

# Node

### **[Electron 18.0.0 Released](https://www.electronjs.org/blog/electron-18-0)**

- 일렉트론 18릴리즈 - 크롬v100, v8 10.0 적용

### **[Postgres.js 3.0: Fast, Full-Featured Postgres Client for Node (and Deno)](https://github.com/porsager/postgres/releases/tag/v3.0.0)**

- sql을 기반으로 하는 쿼리 빌더
- Deno 지원, esm, ts, large object 지원
- 요청 취소

### [Creating Node Docker Images That Build in 2 Seconds (Sort Of)](https://xmorse.xyz/blog/creating-node-js-docker-images-that-build-in-2-seconds-c428aec57fd44a9f93957bdf2ebf4f54)

- 2초만에 빌드되는 노드 도커 이미지 - esbuild

### [Undici 5.0: The Modern HTTP/1.1 Client for Node](https://github.com/nodejs/undici/releases/tag/v5.0.0)


# Javascript

### **[Decorators for ES6 Classes Proposal (Mostly) Reaches Stage 3 at TC39](https://github.com/tc39/proposal-decorators)**

- 데코레이터 조건부로 stage3

### **[React 18 Released](https://reactjs.org/blog/2022/03/29/react-v18.html)**

- [리액트 18 마이그레이션 하는 방법](https://reactjs.org/blog/2022/03/08/react-18-upgrade-guide.html)
- Concurrent React 는 렌더링 도중 멈출 수 있고, 렌더링을 포기 할 수도 있음
- 아직 server component는 개발중이지만, 18.x 에서 초기 버전을 릴리즈 할 예정
- Automatic Batching - setTimeout 콜백에서도 setState의 배치처리
- startTransition API 를 통한 우선순위 조절
- 새로운 Suspense, 새로운 Hooks, 새로운 Strict mode 동작
- 새로운 Client, Server Rendering API

### **[all dropped jQuery as a dependency](https://twitter.com/TheRealNooshu/status/1507346592612896768)**

- 영국 정부 사이트(https://gov.uk)가 jQuery 종속성 제거

### Release

- **[React Testing Library 13](https://github.com/testing-library/react-testing-library/releases/tag/v13.0.0) - react 18 support**
- **[ioredis 5](https://github.com/luin/ioredis/wiki/Upgrading-from-v4-to-v5) -** `@types/ioredis` 제거, default promise만 지원

### **[Locale Aware Sorting in JavaScript](https://elijahmanor.com/byte/js-locale-sort)**

- JS의 기본적인 정렬은 악센트를 포함하지 않음
- compareFunction, Intl.Collator 을 사용하여 정렬하기

### **[How to Use Props in React](https://www.robinwieruch.de/react-pass-props-to-component/)**

- 리액트 props에 대한 설명 - 3년된 글이지만 최근에도 업데이트

### **[14 Linting Rules To Help You Write Asynchronous JS Code](https://maximorlov.com/linting-rules-for-asynchronous-code-in-javascript/)**

- JS 비동기에 대한 14가지 린트 - 비동기를 다룰 때의 주의사항

### **[Visual Studio Code March 2022 Released](https://code.visualstudio.com/updates/v1_66)**

- VSCode 1.66릴리즈
- local history: 로컬 변경사항에 대한 타임라인을 보여주고, 특정 시점으로 이동 가능
- 커서가 있는 라인에 +버튼 추가: 코멘트 추가 버튼
- 터미널 검색 및 하이라이트 기능
- heap profile 수집 및 시각화
- TS 4.7 지원 - 곧 출시될 4.7 릴리즈 초기 지원 포함