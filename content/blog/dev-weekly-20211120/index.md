---
title: dev-weekly 2021-11-20
date: "2021-11-20T09:00:00.000Z"
description: "dev-weekly 2021-11-20"
tags: ["javascript", "node", "css"]
---

# CSS

### **[A Clever Sticky Footer Technique](https://css-tricks.com/a-clever-sticky-footer-technique)**

- 영리하게 footer만드는 방법 6번째 ([지난 5가지](https://css-tricks.com/couple-takes-sticky-footer/))
    
    ```css
    html, body { height: 100%;}
    
    body > footer {
      position: sticky;
      top: 100vh;
    }
    ```
    

### **[Everything You Have to Know About Core Web Vitals](https://calibreapp.com/blog/core-web-vitals)**

- core web vital 에 대한 개요, 중요한 이유 ⇒ 검색 순위에 영향
- 각 지표의 권장 값과 측정 방법 등

### **[Using Position Sticky With CSS Grid](https://ishadeed.com/article/position-sticky-css-grid)**

- grid의 `align-items` 의 디폴트 값은 strech이기 때문에 sticky가 적용되지 않음
- align-items를 start로 바꾸면 sticky 적용

### **[Layout Patterns](https://web.dev/patterns/layout)**

- 공통 인터페이스를 구축하는데 도움이 되는 레이아웃 패턴 모음

### **[Debugging HTML: Accessibility](https://www.htmhell.dev/tips/debugging-html-accessibility/)**

- 브라우저에서 접근성 디버깅하기
    - 크롬과 파이어폭스의 접근성 탭 설명

### **[CSS 3D Cake](https://codepen.io/ShadowShahriar/pen/ZEJerdX)**

# Node

### **[GitHub on npm Ecosystem Security (and a Major Bug They've Fixed)](https://github.blog/2021-11-15-githubs-commitment-to-npm-ecosystem-security/)**

- NPM 2FA

### **[Announcing TypeScript 4.5](https://devblogs.microsoft.com/typescript/announcing-typescript-4-5/)**

- assert
    
    ```tsx
    import obj from "./something.json" assert { type: "json" };
    
    // type is { readonly prop: "hello" }
    let b = { prop: "hello" } as const;
    ```
    

### [https://bundlescanner.com/](https://bundlescanner.com/)

- 사이트 주소를 입력하면 패키지들dml 사이즈와 번들사이즈를 표시
(소스맵 없는곳은 그냥 청크 사이즈)
- 작동방식 - [https://bundlescanner.com/about](https://bundlescanner.com/about)

### **[Electron 16.0.0 Released](https://nodeweekly.com/link/116478/154188e1e3)**

- 크롬 96, V8 9.6 지원

# Javascript

### **[Understanding Why a Build Got 15x Slower with Webpack 5](https://engineering.tines.com/blog/understanding-why-our-build-got-15x-slower-with-webpack)**

- 웹팩에서 CSS in JS 가 느려진 이유
    
    ```tsx
    const dummy = [];
    dummy[Symbol.isConcatSpreadable] = true;
    // Slow path on Node and Chrome
    [].concat([]);
    ```
    

### **[React 18 Enters Beta Stage](https://github.com/reactwg/react-18/discussions/112)**

- 리액트 18 베타 출시. 릴리즈는 2022년 1분기 예정

### Brief

kent c dodds Remix에 합류

- [https://kentcdodds.com/blog/how-i-help-you-build-better-websites](https://kentcdodds.com/blog/how-i-help-you-build-better-websites)

ember 4.0 릴리즈

- [https://github.com/emberjs/ember.js/releases/tag/v4.0.0](https://github.com/emberjs/ember.js/releases/tag/v4.0.0)

netlify $105M 조달하고, 기업가치 $2B로 평가

- [https://www.netlify.com/press/netlify-raises-usd105-million-to-transform-development-for-the-modern-web](https://www.netlify.com/press/netlify-raises-usd105-million-to-transform-development-for-the-modern-web)

### **[MicroDiff: Lightweight, No Dependency Object and Array Comparison](https://javascriptweekly.com/link/116621/4e4af8cb63)**

- 가볍고 빠른 배열, 객체 비교 라이브러리.
- 제로 종속성, TS지원