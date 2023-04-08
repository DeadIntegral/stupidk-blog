---
title: dev-weekly 2021-09-25
date: "2021-09-25T11:00:00.000Z"
description: "dev-weekly 2021-09-25"
tags: ["javascript", "node", "css", "rust"]
---

# CSS

### **[Designing Beautiful Shadows in CSS](https://www.joshwcomeau.com/css/designing-shadows/)**

- 사실적인 그림자를 만드는 기법

# Node

### **[Electron 15.0.0 Released](https://www.electronjs.org/blog/electron-15-0/)**

- 크롬 94, V8 9.4, Node 16.5 적용

# Rust

### **[Rome will be rewritten in Rust](https://rome.tools/blog/2021/09/21/rome-will-be-rewritten-in-rust)**

- 이 프로젝트에 있어서 러스트가 JS보다 더 생산적일 수 있기 때문에 러스트로 다시제작

### **[Goscript is now language feature complete](https://github.com/oxfeeefeee/goscript)**

- 러스트로 작성한 고 스크립트

### **[Optimize Rust binaries size with cargo and Semver](https://oknozor.github.io/blog/optimize-rust-binary-size/)**

- 러스트 바이너리 파일 크기 최적화

# Javascript

### **[Partytown: Run Third-Party Scripts from a Web Worker](https://dev.to/adamdbradley/introducing-partytown-run-third-party-scripts-from-a-web-worker-2cnp)**

- 써드 파티 스크립트가 메인 스레드의 리소스를 점유하는 문제에 대해서
- web worker는 좋은 솔루션이지만 postMessage는 비동기식인 이슈
- 써드 파티 스크립트를 동기적으로 실행할 수 있도록 하는 라이브러리
    - 샌드박싱, 레이아웃 스래싱 감소 등 다양한 목적이 있음
- [https://github.com/BuilderIO/partytown](https://github.com/BuilderIO/partytown)

### **[A Look at 40+ Non-V8 JavaScript Implementations](https://notes.eatonphil.com/javascript-implementations.html)**

- V8 외에 다른 JS 구현체들 및 각각의 지원범위, 구현언어, 런타임, 파서, 릴리즈 등의 정보
- On the JVM
    - Oracle's GraalJS, Mozilla's Rhino, Oracle's Nashorn
- Embeddable
    - Nginx's njs, ChowJS, Artifex's mujs
- Embedded Systems
    - Samsung's Escargot, Espruino, Cesanta's Elk, Cesanta's mJS, Moddable's XS
- Other
    - Facebook's Hermes(RN 엔진), Qt's V4

### **[Introducing Gatsby 4: Now in Beta](https://www.gatsbyjs.com/gatsby-4/)**

- 개츠비 4.0 베타
- 서버 사이드 렌더링 지원
- parallel query running 를 통해 빌드 시간 감소
- [https://v4.gatsbyjs.com/docs/reference/release-notes/migrating-from-v3-to-v4/](https://v4.gatsbyjs.com/docs/reference/release-notes/migrating-from-v3-to-v4/)

### **[V8 release v9.5](https://v8.dev/blog/v8-release-95)**

- 8.1 부터 지원하던 Intl.DisplayNames API 향상
    - calendar, dateTimeField 타입도 지원
    - timeZoneName 옵션 4가지 새로운 값 지원 (GMT-9와 같은 포맷 등)
- WASM Exception Handling
    - 호환되는 툴체인으로 컴파일된 모듈이 V8에서 실행되도록 Wasm EH 프로포절 지원

### **[What's New In DevTools (Chrome 95)](https://developer.chrome.com/blog/new-in-devtools-95/)**

- DevTools 커맨드 메뉴 UI 개선
- DevTools에서 버튼을 통한 이슈 리포트
- 라이트하우스 8.4 릴리즈

### **[What's New in React 18?](https://yagmurcetintas.com/journal/whats-new-in-react-18)**

- 리액트 18 변경사항 요약본

### **[Index Signatures in TypeScript](https://dmitripavlutin.com/typescript-index-signatures/)**

- TS 인덱스 시그니처의 신택스, 주의사항, Record<keys, Type>와 비교

### **[Code2flow: Generate Call Graphs for Dynamic Languages](https://github.com/scottrogowski/code2flow/)**

- JS, Python, Ruby, PHP 지원
- 소스를 AST로 변경하고 함수들을 다이어그램으로 표현해주는 도구