---
title: dev-weekly 2023-03-25
date: "2023-03-25T12:00:00.000Z"
description: "dev-weekly 2023-03-25"
tags: ["javascript", "css", "node"]
---
# CSS

### **[Selecting Previous Siblings with CSS `:has()`](https://tobiasahlin.com/blog/previous-sibling-css-has/)**

- has를 사용하여 특정 형제들 선택하기

# Node

### **[npm Granular Access Tokens Now Generally Available](https://github.blog/changelog/2023-03-21-general-availability-of-granular-access-token-on-npm/)**

- 제한을 가진 액세스 토큰 생성 가능
    - 특정 패키지나 스코프 제한, 특정 조직 제한, 토큰 만료 날짜 셋팅, IP 주소 범위를 기준으로 제한, 토큰의 기능(읽기, 쓰기, 접근)단위 제한 등 제공

### **[Automatic npm Publishing with GitHub Actions and Granular Tokens](https://httptoolkit.com/blog/automatic-npm-publish-gha/)**

- granular token을 사용하여 Github Action을 통한 NPM Publish 자동화하기

### **[Deno 1.32 Released with Enhanced Node Compatibility](https://deno.com/blog/v1.32)**

- 1.32.0 에는 보안 문제가 있으니 1.32.1 사용 권장
- package.json 지원
- NodeJS 호환성 증가, Deno API 변경
- Web API 변경 - URLSearchParams.size제공, WebGPU API 제거
- TS 5.0, V8 11.2 적용

### **[Why We Added `package.json` Support to Deno](https://deno.com/blog/package-json-support)**

- Deno 에서 package.json 지원을 추가한 이유를 설명하는 라이언 달의 글
- Deno 사용자가 Node를 사용할 때 보다 더 효율적으로 작업하도록 지원하기를 희망
    - Node 프로젝트를 Deno에서 직접 실행하기를 원하는 개발자들

# Javascript

### **[Could We Make The Web More Immersive using a Simple Optical Illusion?](https://shopify.github.io/spatial-commerce-projects/WonkaVision/)**

- 웹캠을 이용하여 사용자를 추적하고, 이에 따라 화면의 렌더링을 다르게 하여 입체적으로 보이게 하는 착시
- 이 착시의 제한사항들 - 한쪽 눈 감기

### **[Speeding Up the JavaScript Ecosystem: npm Scripts](https://marvinh.dev/blog/speeding-up-javascript-ecosystem-part-4/)**

- npm cli는 표준 JS 파일이며, 다른 js파일처럼 호출 가능
- `node --cpu-prof $(which npm) run myscript` 를 통해 npm 스크립트의 profile 생성 가능
- 필요하지 않은 기능들을 제거하여 400ms ⇒ 22ms 까지 최적화

### **[Playwright v1.32 – Now with UI Mode](https://github.com/microsoft/playwright/releases/tag/v1.32.0)**

- `npx playwright test --ui`  ui모드

### **[How to Start a React Project in 2023](https://www.robinwieruch.de/react-starter/)**

- Vite, NextJS, Astro 등에 대해 핵심 설명
- 도구별 장단점, 리액트 문서에서 기본값이 아닌 이유등 요약 정리

### **[Tracking the Fake GitHub Star Black Market with Dagster, dbt and BigQuery](https://dagster.io/blog/fake-stars)**

- 깃헙 가짜 스타 시장에 대한 조사
- 가짜 프로필의 조건을 설정해보고 빅쿼리 활용
- 글 게시 후 깃헙의 혹은 가짜 스타 벤더의 조치. 테스트 레포에 스타를 눌렀던 모든 프로필 제거.

### **Release**

- [Docusaurus 2.4](https://docusaurus.io/blog/releases/2.4/)
- [Docs 8.0](https://github.com/dolanmiu/docx/releases/tag/8.0.0)
- [fastify 4.15](https://github.com/fastify/fastify/releases/tag/v4.15.0)
- [hexo 7.0 RC1](https://github.com/hexojs/hexo/releases/tag/v7.0.0-rc1)

### **[A Practical Guide to Getting Started with Astro](https://bejamas.io/blog/practical-guide-to-astro-js-framework/)**

- Asto 를 시작하게 도와주는 방대한 문서
- step by step 으로 cli 및 컨셉에 대한 설명 제공

# ETC

### **[The 'End' of Front-End Development?](https://www.joshwcomeau.com/blog/the-end-of-frontend-development/)**

- AI로 인해 FE가 직업을 잃을것이냐는 질문에 대한 소신발언
- 과거 부터 있던 우려. 2000년대는 워드프레스, 2010년대는 웹플로우, 2020년대는 노코드 도구들
- AI는 훈련 데이터만큼 좋음. 대규모 오픈 소스 코드베이스는 없는데 AI가 대규모 프로젝트를 구축하는 방법은 어떻게 학습할지.
- 주의사항 - LLM을 GPS 네비게이션 취급하지 않기