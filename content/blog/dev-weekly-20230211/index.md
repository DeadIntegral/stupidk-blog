---
title: dev-weekly 2023-02-11
date: "2023-02-11T17:20:00.000Z"
description: "dev-weekly 2023-02-11"
tags: ["javascript", "css", "node"]
---
# CSS

### **[The Guide To Responsive Design In 2023 and Beyond](https://ishadeed.com/article/responsive-design)**

- 고정 크기의 breakpoint의 반응형은 레거시.
- 우리가 레이아웃 디자인을 창의적으로 하지 않는 한 웹은 기본적으로 반응형
- 반응형 디자인의 미래는 전체 페이지를 반응형으로 하는 것이 아닌 컴포넌트에 대한 반응형 CSS를 만들고 브라우저가 자체적으로 스타일 적용할 시기를 결정하는 것.

### **[How to Favicon in 2023: Six files that fit most needs](https://evilmartians.com/chronicles/how-to-favicon-in-2021-six-files-that-fit-most-needs)**

- nanoid 창시자의 Favicon 최적화
- 수십개의 이미지 파일 대신 아이콘5개와 1개의 json파일로 대체하기
    - svg이미지의 svg태그 내에서 미디어 쿼리(`prefers-color-scheme: dark`)를 사용한 대응

### **[CSS Layers for CSS Resets](https://medium.com/appwrite-io/css-layers-for-css-resets-f60f270aa1cd)**

- css layer를 사용하여 css reset과 css normalize와 같은 충돌하는 도구 같이 사용하기

### **[Theme Toggles](https://toggles.dev/classic)**

- 애니메이션 토글 모음
- svg 및 샘플 마크업 제공

### **[Interop 2023 Dashboard](https://wpt.fyi/interop-2023)**

- 브라우저가 각 기술에 대해 웹 표준과 얼마나 일치하는지 백분율로 표시해주는 서비스

# Node

### **[Ada 1.0: Node's Forthcoming New URL Parser](https://github.com/ada-url/ada/releases/tag/v1.0.0)**

- ada가 아니라 Cpp로 작성된 URL 파서 1.0 릴리즈
- WHATWG, nodejs 테스트 슈트 통과

### **[Lambda Cold Starts analysisby maxday](https://maxday.github.io/lambda-perf/)**

- AWS 람다 서버리스 런타임이 시작하는데 얼마나 걸리는지 라이브 데모를 제공하는 페이지

### [On Using Playwright in GitHub Actions](https://radekmie.dev/blog/on-playwright-in-github-actions/)

- github action에 Playwright포함하는 예제
- 테스트에 걸리는 시간 단축을 위한 Playwright 샤드 이용하기
- 종속성 캐시로 빌드 타임 줄이기 - MS 공식 Playwright 이미지 사용하기

### **[Electron 23.0 Released](https://www.electronjs.org/blog/electron-23-0)**

- Chromium 110, V8 11.0, Nodejs 18.12.1 포함. Windows 7/8.1 지원 중단

# Javascript

### **[Speeding Up the JS Ecosystem: It's ESLint's Turn](https://marvinh.dev/blog/speeding-up-javascript-ecosystem-part-3/)**

- ESLint 의 느린 부분들을 최적화하는 포스트
- for of를 for loop으로 변경하기
- AST 노드가 특정 유형(BinaryExpression, VariableDeclaration 등)인지 알고 싶은데 전체를 호출하는것은 낭비.
- `@typescript-eslint/parser` 를 `@babel/eslint-parser`+`@babel/preset-typescript` 로 변경
    - TS AST는 타입 자체를 나타내는 노드도 고려해야함

### **[Ten Web Development Trends in 2023](https://www.robinwieruch.de/web-development-trends/)**

- state of JS 2022를 기반으로 살펴본 2023 웹 개발 트렌드
- 렌더링 패턴의 변화: On-Demand ISR, Streaming SSR.
- Edge to Serverless: Cloud Provider들이 경쟁적으로 TTI 개선 중
- JS Runtime: Deno, Bun

### ****[A HISTORICAL REFERENCE OF REACT CRITICISM](https://www.zachleat.com/web/react-criticism/)****

- 리액트가 나오고부터 지금까지 있었던 비판들 타임라인 정리

### **[Design Patterns in TypeScript](https://refactoring.guru/design-patterns/typescript)**

- TS 디자인 패턴 다이어그램과 설명을 포함한 예제 카탈로그

### **[BlockNote: Notion-Style Block-Based Text Editor](https://github.com/YousefED/BlockNote)**

- Prosemirror, Tiptap 위에 구축한 노션 스타일의 블록 기반 확장 가능한 텍스트 에디터