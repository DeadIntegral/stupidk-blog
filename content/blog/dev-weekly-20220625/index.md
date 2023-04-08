---
title: dev-weekly 2022-06-25
date: "2022-06-25T22:30:00.000Z"
description: "dev-weekly 2022-06-25"
tags: ["javascript", "css", "node"]
---

# CSS

### **[CSS Card Shadow Effects](https://chenhuijing.com/blog/css-card-shadow-effects)**

- 객체가 복사된 것 같은 모습을 `box-shadow` 로 그리는 아티클

### **[ARIA Authoring Practices Guide (APG): Patterns](https://www.w3.org/WAI/ARIA/apg/patterns)**

- w3.org 의 접근성 문서
- ARIA에서 정의한 접근성 의미론을 사용하여 개발하는 방법
- 일반적인 디자인 패턴 및 위젯에 접근성 신택스 적용하는 방법

# Node

### **[Using Web Streams in Node.js](https://2ality.com/2022/06/web-streams-nodejs.html)**

- Axel 박사의 nodejs 에서 웹 스트림 사용하기
- 웹 스트림은 현재 모든 메이저 웹 플랫폼에서 지원하는 스트림의 표준
- nodejs의 웹 스트림에 대해서.
    - 스트림 지원되는 api는 아직 fetch뿐

### **[Puppeteer 15.0: Control Headless Chrome from Node](https://pptr.dev/)**

- Puppeteer 15 릴리즈. (글 작성 시점엔 15.1)
- 크롬 103 (글 작성 시점엔 104), nodejs18 지원

### **[raised $21m in series A funding](https://deno.com/blog/series-a)**

- deno deploy 가 시리즈 A $21M 펀딩
- 리눅스 시스템 콜 대신 JS, WASM을 통한 인터페이스와 보다 빠른 성능의 isolate cloud 제공

# Javascript

### **[Ecma International Approves ECMAScript 2022, But What’s New?](https://2ality.com/2022/06/ecmascript-2022.html)**

- ECMA 2022 승인
- ECMA 2022의 새로운 기능 및 자주하는 질문(JS와의 차이, 설계자, 기능 추가 과정 등)

### **[In Defense of Blocks to Create Localized Scope](https://gist.github.com/getify/712d994419326b53cabe20138161908b)**

- You Dont Know JS 로 유명한 카일 심슨의 스코프 글
    
    ```jsx
    let life = getMeaningOfLife();
    console.log(`The meaning of life: ${life}`);
    // 위 코드 vs 아래 코드
    {
        let life = getMeaningOfLife();
        console.log(`The meaning of life: ${life}`);
    }
    ```
    
- JS에서 어색할 뿐 다른 언어에선 오랜시간 사용하는 방법. 블록으로 래핑하여 얻는 장점들

### **[What the React Team is Working On Now](https://reactjs.org/blog/2022/06/15/react-labs-what-we-have-been-working-on-june-2022.html)**

- 리액트18 릴리즈 이후 리액트 팀이 작업중인 내용

### **[beta of TypeScript 4.8](https://devblogs.microsoft.com/typescript/announcing-typescript-4-8-beta/)**

- —build, —watch, —incremental 성능 향상
- 바인딩 패턴에서 추론 향상

### **[now generally available](https://github.blog/2022-06-21-github-copilot-is-generally-available-to-all-developers/)**

- 깃헙의 코파일럿이 모두에게 오픈, 유료화
- AWS에서 ML 기반 개발 도우미 CodeWhisperer Preview
    - [https://aws.amazon.com/ko/blogs/aws/now-in-preview-amazon-codewhisperer-ml-powered-coding-companion/](https://aws.amazon.com/ko/blogs/aws/now-in-preview-amazon-codewhisperer-ml-powered-coding-companion/)

### **Release**

- Angular eslint v14.0
    - [https://github.com/angular-eslint/angular-eslint/releases/tag/v14.0.0](https://github.com/angular-eslint/angular-eslint/releases/tag/v14.0.0)
- Fastify v4.1
    - [https://github.com/fastify/fastify/releases/tag/v4.1.0](https://github.com/fastify/fastify/releases/tag/v4.1.0)
- React Native 0.69
    - [https://reactnative.dev/blog/2022/06/21/version-069](https://reactnative.dev/blog/2022/06/21/version-069)
    - React 18 지원, 호환되는 헤르메스 엔진을 RN과 같이 출시
    - 브레이킹 체인지 및 주요변화들

### **[Random Notes Around Service Workers Development and Testing](https://mmazzarolo.com/blog/2022-06-18-service-workers-tips-and-tricks/)**

- 서비스 워커 개발 및 테스트와 관련된 몇 가지 팁과 트릭들

### **[main-thread-scheduling 6.0: Consistently Responsive Apps While Staying on the Main Thread](https://github.com/astoilkov/main-thread-scheduling)**

- 웹 워커 대신 requestIdleCallback 를 사용하여 성능 향상(유저 인터랙션 중 메인스레드 작업안함 등)

### **[Reactime 14.0: A Chrome Developer Tool for Time Travel Debugging in React Apps](https://github.com/open-source-labs/reactime/releases/tag/v14.0.0)**

- React 앱의 시간 여행 디버깅 및 모니터링을 위한 크롬 개발자 도구 Reactime 14.0 릴리즈
- 경로별 성능 측정항목 필터링, React Router 지원

# ETC

### **[Stackoverflow 2022 survey](https://survey.stackoverflow.co/2022/)**

- 코딩 경험 50년이상 개발자 0.34%(240명), 전문 개발 경험 50년 이상 0.11%(55명)
- 가장 선호하는 IDE는 VSCode(중복허용 74%, 2위 비주얼 스튜디오 32%)