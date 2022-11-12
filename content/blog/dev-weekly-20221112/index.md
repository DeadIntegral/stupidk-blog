---
title: dev-weekly 2022-11-12
date: "2022-11-12T17:00:00.000Z"
description: "dev-weekly 2022-11-12"
tags: ["javascript", "css", "node"]
---

# CSS

### **[A Couple Changes Coming in Chrome 108](https://css-tricks.com/a-couple-changes-coming-in-chrome-108)**

- 크롬108 부터는 img, video, canvas가 overflow시키던 것 변경
- 안드로이드 크롬에서 키보드가 표시될 때 레이아웃 뷰포트가 변경되지 않음

### **[The Shared Element Transition API is FLIPping Cool](https://chriscoyier.net/2022/10/21/the-shared-element-transition-api-is-fliping-cool)**

- Shared Element Transition 으로 Fliping 애니메이션 만들기

### **[Browser Logos](https://github.com/alrra/browser-logos)**

- 배경이 투명한 고해상도 브라우저 로고 모음. 과거부터 지금까지의 로고들 존재

# Node

### **[Node.js Security Best Practices](https://nodejs.org/en/docs/guides/security/)**

- Nodejs 오피셜 새로운 보안 가이드
    - 각 공격 예시와 보안 제안
    
    ```jsx
    const a = {"a": 1, "b": 2};
    const data = JSON.parse('{"__proto__": { "polluted": true}}');
    
    const c = Object.assign({}, a, data);
    console.log(c.polluted); // true
    
    // Potential DoS
    const data2 = JSON.parse('{"__proto__": null}');
    const d = Object.assign(a, data2);
    d.hasOwnProperty('b'); // Uncaught TypeError: d.hasOwnProperty is not a function
    ```
    

### **[Hapi 21: A Simple, Secure Node App Framework](https://github.com/hapijs/hapi/releases/tag/v21.0.0)**

- Hapi 21 릴리즈.  Node18 지원 및 ESM호환.
- Nodejs v12 지원 중단

# Javascript

### **[Rome v10: Rust-Powered JS Linting and Formatting](https://rome.tools/blog/2022/11/08/rome-10/)**

- Rust로 재작성 후 첫 스테이블 릴리즈.
- 빠르고 강력한 새로운 린터 - 오류표시, 디테일한 오류표시

### **[Gatsby 5.0: The Fastest Gatsby Yet](https://www.gatsbyjs.com/blog/gatsby-5/)**

- slice: 공유 컴포넌트는 한번만 빌드. 90% 성능 향상
- Partial Hydration: React Server Component를 기반
- Script Component: 다양한 전략을 갖고있는 Script 삽입 기능(idle 타임 로드, 파티타운 사용 등)
- Head API: SEO에 대한 기본 지원 제공. (react helmet보다 쉽고 빠르고 작음)
- GraphiQL v2: GQL 통합 개발 환경
- [릴리즈 노트](https://www.gatsbyjs.com/docs/reference/release-notes/v5.0/)
- [4 to 5 마이그레이션 가이드](https://www.gatsbyjs.com/docs/reference/release-notes/migrating-from-v4-to-v5/)

### **[GitHub Blocks](https://blocks.githubnext.com/)**

- github block을 이용해 readme를 동적으로 작성 가능

### **[Parcel 2.8](https://parceljs.org/blog/v2-8-0/)**

- 새로운 번들 알고리즘: 자동 코드 분할
- HMR 리빌드 성능: 종속성이 변경된것이 아니라면 전체 리빌드 대신 부분적으로 변경, 소켓으로 변경사항 전달
- 트리쉐이킹 개선

# ETC

### ****[Hey, GitHub](https://githubnext.com/projects/hey-github)****

- 음성으로 깃헙에게 말하면, 코파일럿이 코딩해주는 도구