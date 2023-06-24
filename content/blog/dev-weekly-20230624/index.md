---
title: dev-weekly 2023-06-24
date: "2023-06-24T12:00:00.000Z"
description: "dev-weekly 2023-06-24"
tags: ["javascript", "css", "node"]
---
# CSS

### **[What exactly is :root pseudo-element in CSS?](https://www.youtube.com/watch?v=lXUS5E4gqV0)**

- :root vs HTML 차이. :root는 svg와 같이 html 요소가 아닌 것에도 영향.

### **[Optimus Prime with CSS Transform](https://codepen.io/jh3y/pen/MWzwamV)**

- HTML, CSS만으로 만든 변신 가능한 옵티머스 프라임

# Node

### **[Node.js Security Progress Report – First Response Time Down to 8 Hours, New Security Release Announced](https://openjsf.org/blog/2023/06/16/node-js-security-progress-report-first-response-time-down-to-8-hours-new-security-release-announced/)**

- Nodejs의 보안 보고서 8시간까지 단축.
- 목표 시간은 48시간이지만, 빌드 프로세스에 따라 변동. 8시간은 훌륭한 응답.

### **[A Complete Visual Guide to Understanding the Node.js Event Loop](https://www.builder.io/blog/visual-guide-to-nodejs-event-loop)**

- NodeJS의 비동기. libuv와 이벤트 루프에 대한 개요, 작동 순서에 대한 설명
- 이벤트 루프 이해를 위한 비쥬얼 가이드 시리즈 1편.

# Javascript

### **[Announcing Svelte 4](https://svelte.dev/blog/svelte-4)**

- 4년만에 메이저 버전 업데이트.
- 하이드레이션 번들 사이즈 감소, 성능 향상. 패키지 크기 감소(2.8MB), 종속성 수 감소(61 → 16).
- [svelte.dev](http://svelte.dev) 사이트 개편.
- 스벨트5는 컴파일러와 런타임을 다시 작성. 4는 일부 레거시 지원 중단 등 5를 위한 토대.

### **[Deno Fresh 1.2 Release](https://deno.com/blog/fresh-1.2)**

- Deno팀에서 Fresh 오픈소스 후 관리를 잘 못했지만, Preact의 창시자를 새로운 관리자로 발탁.
- renderAsync hook 지원. JSX를 islands로 전달하고, islands들을 중첩가능하도록 지원.

### **[Simple React Component That Makes Titles More Readable](https://react-wrap-balancer.vercel.app/)**

- 제목의 길이를 적절하게 만들어주는(여러 줄 일 때 각 행당 글자를 조정하는) 도구.
- 1KB Gzipped, O(log n) 성능, 레이아웃 시프트 오프, 스트리밍 SSR 지원 등.

### **[Migrating Netflix to GraphQL Safely](https://netflixtechblog.com/migrating-netflix-to-graphql-safely-8e1e4d4f1e72)**

- 넷플릭스의 모바일 앱을 다운타임 없이 GraphQL로 마이그레이션
- AB테스팅 전략 - 기능적 요구사항과 비기능적 요구사항 구분, 멱등성
- 기술은 끊임없이 변화하고, 중요한것은 마이그레이션을 여부가 아니라, 다운타임 없이 적시에 안전하게 마이그레이션 할 수 있는가.

### Release

- **[React Native 0.72 - Symlink Support, Better Errors, and more](https://reactnative.dev/blog/2023/06/21/0.72-metro-package-exports-symlinks)**
- **[tesseract.js 4.1.1](https://github.com/naptha/tesseract.js/releases/tag/v4.1.1)**
- **[testcafe v3.0.0](https://github.com/DevExpress/testcafe/releases/tag/v3.0.0)**

# ETC

### **[New W3C website deployed](https://www.w3.org/news/2023/new-w3c-website-deployed/)**

- W3C 홈페이지 UI 변경

### **[W3C advances technology to streamline payment authentication](https://www.w3.org/press-releases/2023/spc-cr/)**

- 웹 결제 시 사용자 인증 간소, 결제 보안 강화하는 새로운 브라우저 기능 표준화 이정표 발표
- 판매자, 은행, 결제 서비스 제공업체, 카드 네트워크 등이 고객 인증의 마찰을 줄이고, 사용자 동의에 대한 암호화된 증거 생성 가능

### **[Introducing HTTP/3 Prioritization](https://blog.cloudflare.com/better-http-3-prioritization-for-a-faster-web/)**

- 테스트에서 LCP를 37%까지 감소
- 기존에는 defer스크립트와 LCP 이미지가 우선순위가 같은 우선순위로 요청되었을 때, 스크립트가 전송되고 CPU 블록킹이 걸리고 이후 이미지가 렌더링. 이 기술은 스크립트 전송을 중지하고 이미지를 먼저 전송한뒤 js파일을 이어서 전송.
- 빠른 페이지 로드를 위해 Extensible Priorities 신호를 보고 우선순위 결정 알고리즘을 통해 응답 데이터를 보내는 좋은 방법을 결정.

### **[Fit-to-Width Text](https://kizu.dev/fit-to-width-text/)**

- Scroll-driven animation을 사용하여 순수 CSS만으로 width에 fit하도록 font size가 조정하기
- 크롬 기준 116부터 사용 가능

### **[MS Clarity가 영구 무료인 이유](https://clarity.microsoft.com/pricing)**

- 사용자 동작과 관련된 대량의 익명 데이터를 처리하여 기계 학습 모델을 파악 및 개선.
- MS가 데이터를 수집하는 방법.