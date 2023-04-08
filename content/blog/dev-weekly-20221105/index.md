---
title: dev-weekly 2022-11-05
date: "2022-11-05T14:00:00.000Z"
description: "dev-weekly 2022-11-05"
tags: ["javascript", "css", "node"]
---
# CSS

### **[Let’s Talk About Web Components](https://bradfrost.com/blog/post/lets-talk-about-web-components)**

- 웹 컴포넌트에 대한 고찰

### **[Fancy Image Decorations: Outlines and Complex Animations](https://css-tricks.com/fancy-image-decorations-outlines-and-complex-animations)**

- 래퍼없이 img 요소만 사용하여 이펙트 넣기
- 음수 outline을 활용한 트릭

# Node

### **[Nov 3 2022 Security Releases](https://nodejs.org/en/blog/vulnerability/november-2022-security-releases/)**

- [https://www.openssl.org/news/secadv/20221101.txt](https://www.openssl.org/news/secadv/20221101.txt) 에서 안내하는 OpenSSL 이슈 처리
- 14.x, 16.x, 18.x, 19.x 릴리즈

### **[On Rust and Its Relationship with Node](https://sprkl.dev/performance-rust-node-js/)**

- Node에 Rust를 통합했을때의 이점들
- 활발한 커뮤니티, WASM을 통한 통합 등

### **[The Remix Project is Joining Shopify](https://shopify.engineering/remix-joins-shopify)**

- Remix 프로젝트가 Shopify 에 합류
- shopify는 hydrogen을 포함한 다양한 제품에서 Remix를 사용

### **[How to Build, Test, and Publish a TypeScript npm Package in 2022](https://www.strictmode.io/articles/build-test-and-publish-npm-package-2022)**

- TS node module을 생성, Jest 붙이기, npm publish 까지의 간단한 예제

### **[directory-serve: Serve a Local Directory over HTTP](https://github.com/cube-root/directory-serve)**

- `npx directory-serve .` 를 실행하면 현재 디렉토리의 파일을 웹 기반 인터페이스로 표시하는 도구

# Javascript

### **[Is Turbopack Really 10x Faster Than Vite?](https://github.com/yyx990803/vite-vs-next-turbo-hmr/discussions/8)**

- 에반유의 터보팩 벤치마크에 관한 고찰
- 콜드 스타트에서는 10배 차이를 찾을 수 없어 HMR로 비교
    - Next가 리액트 서버 컴포넌트 사용하는지 여부와, Vite가 Babel 대신 SWC 사용하는지 여부가 중요
    - JSX 변환은 빌드 툴의 기능이 아님. Vite는 바벨 쓰는데 터보팩은 SWC를 이용 (둘은 20~70배 성능차이가 있음). SWC 적용해보니까 성능차이가 크지 않음
- vercel 의 벤치마크 방법론 - [https://turbo.build/blog/turbopack-benchmarks](https://turbo.build/blog/turbopack-benchmarks)
- vercel은 모든 규모를 지원할 수 있다를 목표로 설계. 기업규모 1~10 중 6~7정도면 컴포넌트 3만개

### **[Announcing TypeScript 4.9 RC](https://devblogs.microsoft.com/typescript/announcing-typescript-4-9-rc/)**

- `satisfies` 오퍼레이터 - 표현식 유형이 일부 유형과 일치하는지 확인 가능한 오퍼레이터
- 클래스에 Auto Accessor 추가, NaN 비교 기능, file watching은 이제 file system event 사용 등
- 성능 향상 - 모든 syntax node에서 switch 문 대신 function table lookup을 사용하도록 재작성
- 브레이킹 체인지 - Promise.resolve, JS Emit 등

### **[Use TypeScript by default for new applications](https://github.com/facebook/react-native/pull/35165)**

- React Native에서 새 앱 템플릿을 Flow에서 TS로 변경

### **[What's new in Svelte: November 2022](https://svelte.dev/blog/whats-new-in-svelte-november-2022)**

- 스벨트, 스벨트킷의 현 상태 업데이트

### **Release**

- [Redux Toolkit 1.9](https://github.com/reduxjs/redux-toolkit/releases/tag/v1.9.0)
- [VSCode October 2022 (version 1.73)](https://code.visualstudio.com/updates/v1_73)
- [Forge 6.0](https://www.electronforge.io/) **-** https://github.com/electron/forge/releases/tag/v6.0.0
    - 일렉트론 올인원 패키지

### **['Your Next.js Bundle Will Thank You'](https://renatopozzi.me/articles/your-nextjs-bundle-will-thank-you)**

- Nextjs에서 번들 사이즈 분석 및 오작동중인 청크에 대한 해결책들
- Terser가 모듈 export가 사용되는지 여부를 결정할 수 없어 트리쉐이킹이 되지 않는 이슈

### **[Building an Accessible Tooltip Component](https://web.dev/building-a-tooltip-component/)**

- 접근성을 고려한 툴팁 컴포넌트 만들기

# ETC

### **[Introducing the Ask Wizard: Your guide to crafting high-quality questions](https://stackoverflow.blog/2022/10/27/introducing-the-ask-wizard-your-guide-to-crafting-high-quality-questions/)**

- 스택오버플로에 고퀄리티 질문을 할 수 있도록 Ask Wizard 추가