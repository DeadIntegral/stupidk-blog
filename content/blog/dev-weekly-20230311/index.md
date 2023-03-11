---
title: dev-weekly 2023-03-11
date: "2023-03-11T11:30:00.000Z"
description: "dev-weekly 2023-03-11"
tags: ["javascript", "css", "node"]
---

# CSS

### [An End to Typographic Widows on the Web](https://clagnut.com/blog/2424/)

- `text-wrap:balance` 크롬 카나리에 추가.
- 엔진이 판단하여 적정한 시점에 개행

# Node

### **[Feathers 5: The API and Real-Time App Framework](https://blog.feathersjs.com/introducing-feathers-5-the-api-and-real-time-application-framework-101ae2deaaeb)**

- 전체 코드를 TS로 재작성. DB어댑터, 코어, CLI 등 전부 TS
- Koa에 대한 지원 추가

### **[Ink 4.0: React, but for Building Interactive CLI Apps](https://github.com/vadimdemedes/ink/releases/tag/v4.0.0)**

- Ink 4.0 릴리즈
- pure ESM (commonJS 지원 종료), node 14.16 이상 필요, react 18 이상 필요
- react-devtools-core가 옵셔널 피어 디펜던시로 변경

### **[Introducing nsuv: A C++ Wrapper Around `libuv`](https://nodesource.com/blog/intro-nsuv)**

- 이벤트 루프 기반의 하는 비동기 IO를 지원하는 다중 플랫폼  라이브러리 libuv의 래퍼 nsuv 제작 리뷰
- 런타임 오버헤드는 제로에 가깝게 유지하고, libuv API 구조를 모방하여 인지 부하를 줄임

# Javascript

### [2023 Web Framework Performance Report](https://astro.build/blog/2023-web-framework-performance-report/)

- astro 에서 작성한 웹 프레임워크 리포트. Astro, SvelteKit, Gastby, Remix, WordPress, Next, Nuxt의 FID, CLS, LCP, INP, LightHouse 스코어 등에 대한 통계
- 용량 제한, private 페이지 접근 불가(백오피스 등), 레거시 웹 사이트로 인한 수명 영향등의 지표적 한계 설명
- 참조링크 - [https://httparchive.org/](https://httparchive.org/)

### **[TypeScript's Migration to Modules](https://devblogs.microsoft.com/typescript/typescripts-migration-to-modules/)**

- TS 5.0 의 주요 변경 사항 중 하나는 인프라. ECMA모듈 사용. CommonJS가 작성한 API를 계속 제공
- TS는 TS로 만들어서 개발 경험을 일해하는데 도움이 됐지만, 모듈 방식이 아니라 네임스페이스 방식으로 개발. 이 부분에 대한 DX를 놓침.
- 벤치마크 결과 end to end 는 줄었지만 파싱 속도가 느려짐.
- let, const는 선언 전에 참조가 안되서 엔진이 캡처할 때 가드 삽입. 이로인한 오버헤드가 발생하고 바벨을 돌려보니 성능 향상. 몇 군데에서 no var ESLint를 끄고 var로 작성

### **[jQuery 3.6.4 has been released](https://blog.jquery.com/2023/03/08/jquery-3-6-4-released-selector-forgiveness/)**

- CSS가 지원하는 신택스 `:has(:contain)` 과 같은 구문을 사용할 때 jQuery에서 에러를 뱉지 않도록 수정.

### Release

- [Jest 29.5](https://github.com/facebook/jest/releases/tag/v29.5.0) - 실행 순서 셔플하는 기능 추가
- [SWR 2.1](https://github.com/vercel/swr/releases/tag/v2.1.0) - `useSWRSubscription` hook 추가
- **[ClearScript 7.4](https://github.com/microsoft/ClearScript/releases/tag/7.4.0) -** .net 앱에 JS 스크립팅 추가하는 도구 (V8, JScript, VBScript 지원)