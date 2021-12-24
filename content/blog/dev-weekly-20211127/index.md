---
title: dev-weekly 2021-11-27
date: "2021-11-27T10:00:00.000Z"
description: "dev-weekly 2021-11-27"
tags: ["css", "node", "javascript"]
---

# CSS

### **[My Custom CSS Reset](https://www.joshwcomeau.com/css/custom-css-reset)**

- css reset을 모던 브라우저에 맞춰서 커스텀
    
    ```css
    img, picture, video, canvas, svg {
      display: block;
      max-width: 100%;
    }
    ```
    
    ```css
    input, button, textarea, select {
      font: inherit;
    }
    ```
    

### **[Control Layout in a Multi-Directional Website](https://css-tricks.com/control-layout-in-a-multi-directional-website)**

- CSS를 사용하여 다국어 랜딩 페이지 만들기
- `:lang` pseudo-class를 사용하여 writing-mode 변경(세로 쓰기)

# Node

### **[Seven Ways to Improve Node Performance at Scale](https://blog.appsignal.com/2021/11/24/7-ways-to-improve-nodejs-performance-at-scale.html)**

- 프로파일링, 모니터링, 타임아웃, 캐싱, 클러스터링, 로드밸런싱 등에 대한 조언

# Javascript

### **[Remix: A Newly Open Sourced React-Based Framework for Web Apps](https://remix.run/)**

- sponsorware로 제공되던 Remix가 $3M 펀딩을 받으며 프로젝트 시작

### **[Vercel, Creator of Next.js, Raises $150M](https://vercel.com/blog/vercel-funding-series-d-and-valuation)**

- $2.5B 가치로 $150M 추가조달. 총 투자금액 $313

### **[Prettier 2.5 Released: Now with TypeScript 4.5 and MDX v2 Support](https://prettier.io/blog/2021/11/25/2.5.0.html)**

- TS 4.5의 modifier import, private field presence, import Assertions 등 지원
- html class어트리뷰트 개행제거 - tailwind등의 사용자를 위한 기능이었지만 제거

### **[AWS Free tier big change](https://aws.amazon.com/ko/blogs/aws/aws-free-tier-data-transfer-expansion-100-gb-from-regions-and-1-tb-from-amazon-cloudfront-per-month/)**

- cloud front의 트래픽은 월 최대 1TB에 대해 무료, 가입 후 12개월 제한 제거
- http request 200만 ⇒ 1000만건에 대해 무료
- cloud front function call에 대해 12개월 제약 제거, 월 200만건 무료

### Release ses

Chalk 5.0

- [https://github.com/chalk/chalk/releases/tag/v5.0.0](https://github.com/chalk/chalk/releases/tag/v5.0.0)

React Redux v8 Beta

- [https://github.com/reduxjs/react-redux/releases/tag/v8.0.0-beta.0](https://github.com/reduxjs/react-redux/releases/tag/v8.0.0-beta.0)

### **[https://www.joshfinnie.com/blog/using-webassembly-created-in-rust-for-fast-react-components/](https://www.joshfinnie.com/blog/using-webassembly-created-in-rust-for-fast-react-components/)**

- 리액트 컴포넌트에 Rust wasm 사용하기 튜토리얼

### **[PickBetterPack: Discover Similar Packages from `package.json` Dependencies](https://pickbetterpack.com/)**

- package.json의 의존성에 있는 도구들과 유사한 도구들을 찾아주는 서비스

### **[use-prosemirror: Use the ProseMirror Editor in React Easily](https://github.com/dminkovsky/use-prosemirror)**

- ProseMirror 를 리액트로 쉽게 사용하도록 만든 도구