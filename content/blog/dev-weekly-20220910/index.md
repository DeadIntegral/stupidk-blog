---
title: dev-weekly 2022-09-10
date: "2022-09-10T23:27:00.000Z"
description: "dev-weekly 2022-09-10"
tags: ["javascript", "css", "node",]
---
# CSS

### **[Hacking CSS Animation State and Playback Time](https://css-tricks.com/hacking-css-animation-state-and-playback-time)**

- CSS Only game을 보고 만들어보는 CSS 애니메이션
- 웹의 애니메이션은 stateless. 그 안에서 슬로우 모션 및 다시 재생 제어하기
- CSS로 가능한 최대치, JS를 최소화해서 만드는 애니메이션

### **[How To Improve Largest Contentful Paint for Faster Load Times](https://calibreapp.com/blog/largest-contentful-paint)**

- LCP를 최적화 하는 방법
- [https://www.searchenginejournal.com/ranking-factors/core-web-vitals/](https://www.searchenginejournal.com/ranking-factors/core-web-vitals/) 구글의 웹 바이탈 영향

# Node

### **[An Overview of Node's Architecture, Event Loop, and More](https://2ality.com/2022/09/nodejs-overview.html)**

- Dr. **Axel 의 Nodejs 아키텍처**
- nodejs platform, event loop, libuv(async io cross platform), escape main thread
    - 브라우저와는 다른 nodejs 의 이벤트 루프

### **[Rewriting Tests from Cypress to Playwright with AI](https://contra.com/p/PWBcPYZc-rewriting-tests-from-cypress-to-playwright-using-gpt-3)**

- cypress에서 playwright로 마이그레이션하는 과정
- 코파일럿은 때때로 작동하지 않거나, 프로젝트가 커지면서 제안을 잘 못하거나 하는 등 이슈가 발생, 코파일럿은 GPT3 + codex니까 GPT3를 직접 이용하기로 결정

### **[GradeJS: Scan Production Webpack Bundles for Modules Within](https://gradejs.com/)**

- 원본 코드에 액세스 하지 않더라도 프로덕션 번들을 분석해주는 도구
- 사이트를 입력하면 사용된 npm 패키지들을 분석하고, 사용된 패키지별 버전, 용량등을 표기

### **[Deploying a Node App and Postgres Database to Fly.io](https://simonplend.com/deploying-a-node-app-and-postgres-database-to-fly-io/)**

- Heroku를 대신할 배포 플랫폼 [fly.io](http://fly.io)
- 호스팅 플랫폼에 배포

# Javascript

### **[Ryan Dahl Asks Oracle to Release the 'JavaScript' Trademark](https://tinyclouds.org/trademark)**

- nodejs의 창시자 라이언 달이 오라클에 JS상표권에 대해 공개하자는 글

### **[Introducing Signals: A Reactive State Primitive That's Fast By Default](https://preactjs.com/blog/introducing-signals/)**

- preact 상태 관리 도구 signal 소개
- 프레임워크에 수동으로 통합 할 필요 없는 도구 (react 바깥에서 작동)

### **[Announcing React Native 0.70](https://reactnative.dev/blog/2022/09/05/version-070)**

- RN 0.70 릴리즈
- 기본 JS엔진 헤르메스로 변경
- 새로운 아키텍처와 새 문서

### **[History of JavaScript on a Timeline](https://blog.risingstack.com/history-of-javascript-on-a-timeline/)**

- JS의 역사 타임라인 - 넷스케이프, 브렌든아이크, MS JScript 부터 TS, ECMA2021에 이르기까지

### Release

- [https://nextjs.org/blog/next-12-3](https://nextjs.org/blog/next-12-3)
- [https://github.com/emberjs/ember.js/releases/tag/v4.7.0](https://github.com/emberjs/ember.js/releases/tag/v4.7.0)
- [https://deno.com/blog/fresh-1.1](https://deno.com/blog/fresh-1.1)

### **[TIL You Can Access a User’s Camera with Just HTML](https://austingil.com/html-capture-attribute/)**

- input capture를 이용해 카메라 접근하기
- 지원하지 않는 모바일 브라우저에서는 file 로 폴백

### **[JSON Hero: A Beautiful JSON Viewer](https://javascriptweekly.com/link/128612/4e4af8cb63)**

- JSON 데이터(혹은 JSON을 반환하는 URL)를 넣으면 이쁘게 보여주는 도구
- [https://jsoncrack.com/](https://jsoncrack.com/) 이 차트로 보여준다면, hero는 각 데이터의 미리보기 및 타입별로 파싱

### **[DgrmJS: A Library for Creating SVG Diagrams](https://github.com/AlexeyBoiko/DgrmJS)**

- 다이어그램 에디터를 제공하는 도구
- gzip 3.3kb, minified 10.4kb