---
title: dev-weekly 2022-07-30
date: "2022-07-30T16:00:00.000Z"
description: "dev-weekly 2022-07-30"
tags: ["javascript", "node", "css"]
---

# 2022-07-30

# CSS

### **[The CSS Behind Figma](https://ishadeed.com/article/figma-css)**

- 피그마에서 사용한 Grid와 Flex
- 그리드의 한 칸을 작게 설정하고 반복시킨 뒤 메뉴 하나가 여러 칸을 점유하도록 하는 방식

### **[Use Firefox for Accessibility Testing](https://www.a11yproject.com/posts/using-firefox-for-accessibility-testing)**

- 파이어폭스의 a11y 도구들
- 시뮬레이션, 탭 순서, 검사 및 프로퍼티 패널
- Wave extension, axe Devtools extension, etc

# Node

### **[Introducing *Even More* Security Enhancements to npm](https://github.blog/2022-07-26-introducing-even-more-security-enhancements-to-npm/)**

- 간소화된 로그인 및 퍼블리싱 (8.15.0 이상에서 제공. 9에서 디폴트)
    
    ```jsx
    npm login --auth-type=web
    npm publish --auth-type=web
    ```
    
- 깃헙, 트위터 계정등을 NPM에 연결
- `npm audit signature` (8.13.0 이상에서 제공)

### **[Using Rust for Writing Node Modules](https://blog.techfund.jp/p/using-rust-for-writing-nodejs-modules/)**

- Rust로 노드 모듈 만들기
- NodeJS 바인딩과 직접 통합
    - rust에서는 nj-cli로 빌드

### **[serverless-bundle 5.4: Optimized Packages for Config-Free ES6 and TypeScript Node.js Lambda Functions](https://github.com/AnomalyInnovations/serverless-bundle)**

- 내부적으로 serverless-webpack을 사용

### ETC

- [https://github.com/sindresorhus/got/releases/tag/v12.3.0](https://github.com/sindresorhus/got/releases/tag/v12.3.0)
- [https://github.com/fastify/fastify/releases/tag/v4.3.0](https://github.com/fastify/fastify/releases/tag/v4.3.0)

# Javascript

### **[Douglas Crockford: "The best thing we can do today to JavaScript is to retire it."](https://evrone.com/douglas-crockford-interview)**

- JSON 창시자 더글라스 크락포드 인터뷰.
- JS는 다른 공룡 언어와 마찬가지로 발전을 가로막는 장벽. 다음 언어에 집중해야함.

### **[examples of larger production-grade open source React apps](https://maxrozen.com/examples-of-large-production-grade-open-source-react-apps)**

- 프로덕션급 오픈 소스 리액트 엡 예제 모음
- Jira Clone, real world, cypress realworld, AST Explorer, Excalidraw, Sentry, Grafana, etc

### **[Extract Parameter Types from String Literal Types with TypeScript](https://lihautan.com/extract-parameters-type-from-string-literal-types-with-typescript/)**

- TS 타입에 대한 가이드 문서
- Conditional Type, Template Literal Type 에 대한 가이드