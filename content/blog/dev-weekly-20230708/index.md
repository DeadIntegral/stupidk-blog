---
title: dev-weekly 2023-07-08
date: "2023-07-08T15:55:00.000Z"
description: "dev-weekly 2023-07-08"
tags: ["javascript", "css", "node", "etc"]
---
# CSS

### **[Zero-Runtime CSS with Vanilla Extract](https://www.telerik.com/blogs/zero-runtime-css-vanilla-extract)**

- CSS-in-JS의 문제점 및 Vanilla Extract 장점 소개

# Node

### **[Avoid Fastify's reply.raw and reply.hijack Despite Being A Powerful HTTP Streams Tool](https://www.lirantal.com/blog/avoid-fastify-reply-raw-and-reply-hijack-despite-being-a-powerful-http-streams-tool)**

- fastify에서 reply.raw, reply.hijack를 사용할 때 발생할 수 있는 문제점
- readableStream 를 사용하는 대안 제시

### **[Automize: The missing Chrome Devtools Element Selector](https://automize.dev/)**

- 특정 엘리먼트의 고유한 셀렉터를 뱉어주는 도구.
- Puppeteer, Playwright, Cypress, Selenium과 같은 도구와 호환

### **[Deno 1.35: A fast and convenient way to build web servers](https://deno.com/blog/v1.35)**

- `Deno.serve()` 이제 스테이블하고 성능도 향상.
- npm, node 호환성 개선
- semver를 포함하여 표준 라이브러리 변경

# Javascript

### **[Announcing TypeScript 5.2 Beta](https://devblogs.microsoft.com/typescript/announcing-typescript-5-2-beta/)**

- TS 5.2 베타.
- using과 explicit resource management. 생성할 때 소멸자도 같이 정의하여 리소스 관리를 용이하게 해주는 문법
- Decorator Metadata
- 익명 튜플 지원

### **[RegExp v flag with set notation and properties of strings](https://v8.dev/features/regexp-v-flag)**

- 정규식에 v 플래그 지원. 2022년에 시작했지만 크롬 112, 사파리 17 부터 지원
- 유니코드 문자 속성에 접근 권한 - 그리스어 가져오기 (ex: `/\p{Script_Extensions=Greek}/u;`)
- `const re = /^\p{RGI_Emoji}$/v;` u플래그와 다르게 조합된 이모지도 접근

### **[Understanding SVG Paths](https://www.nan.fyi/svg-paths)**

- SVG 의 표현법을 시각적으로 표현하여 이해를 돕는 가이드

### **[An Introduction to the View Transitions API](https://www.sitepoint.com/view-transitions-api-introduction/)**

- 페이지 내에서 애니메이션 전환을 하는 예제로 View Transition API 소개
- 파이어폭스와 사파리는 구현 계획이 없지만, 애니메이션만 추가하면 상관없을 것.

### **[Remotion 4.0](https://www.remotion.dev/blog/4-0)**

- React로 영상 편집하는 도구 Remotion 4.0 릴리즈
- cli 대신 버튼을 통한 렌더링, Rust 바이너리 파일, FFmpeg 내장, OffthreadVideo 지원
- WebP, PDF파일 생성 지원, ES Module 지원

### **[JavaScript Gom Jabbar](https://frantic.im/javascript-gom-jabbar/)**

- Gom jabbar는 듄 세계관에서 극심한 고통을 주는 도구. 제목은 고통스러운 JS 경험을 은유하는 단어.
- package.json을 열어보면 version, main, browser, type, lint, yarn, 수많은 변형, 레졸루션, 디펜던시, engine 등 알아야 할 것이 너무 많다는 글

### **[MATHLIVE: A WEB COMPONENT FOR MATH INPUT](https://cortexjs.io/mathlive/)**

- 수학 콘텐츠 조판의 표준인 Tex 레이아웃 알고리즘 JS 구현체
- 수학 기호, 행렬, 화학 방정식, 매크로 등을 포함한 800개 이상의 Tex 커맨드 지원

# ETC

### **[115.0 Firefox Release](https://www.mozilla.org/en-US/firefox/115.0/releasenotes/)**

- Windows 7, 8 의 사용자가 받아볼 수 있는 마지막 메이저 버전
- 마이그레이션 - 크롬으로부터 기본 브라우저를 변경 시 저장된 결제 수단도 임포트
- H264 비디오 디코딩을 할 수 없는 플랫폼에서도 Cisco의 OpenH264 플러그인으로 대체

### **[Happy 50th birthday, Ethernet](https://blog.apnic.net/2023/06/29/happy-50th-birthday-ethernet/)**

- 이더넷의 50번째 생일을 맞이하여 이더넷이 어떻게 발전해왔는지 설명

### **[Vite 4.4.0](https://github.com/vitejs/vite/blob/main/packages/vite/CHANGELOG.md#440-2023-07-06)**

- 실험적인 Lightning CSS 지원. esbuild 0.18 적용.
- create-vite 에 solid와 Qwik 템플릿 추가. 문서 한국어 번역([https://ko.vitejs.dev/](https://ko.vitejs.dev/)).
- 글 작성 시점엔 4.4.2 릴리즈