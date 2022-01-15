---
title: dev-weekly 2022-01-15
date: "2022-01-15T10:00:00.000Z"
description: "dev-weekly 2022-01-15"
tags: ["javascript", "node", "css"]
---

# CSS

### **[Writing Better CSS](https://www.aleksandrhovhannisyan.com/blog/writing-better-css)**

- `:is`
    
    ```jsx
    .nav-link {
      &:focus,
      &:hover,
      &[aria-current="page"] {}
    }
    // .nav-link:is(:focus, :hover, [aria-current="page"]) {}
    
    .token.tag,
    .token.keyword,
    .token.someOtherThing {}
    // .token:is(.tag, .keyword, .someOtherThing) {}
    ```
    
    - Forgiving Selector Parsing - safari는 지원 안함
- `clamp`
    
    ```jsx
    .element {
      property: clamp(<min>, <preferred>, <max>);
    }
    ```
    
- `aspect-ratio`, `where`, `margin-inline-start`, `gap`

### **[CSS in 2022](https://www.bram.us/2021/12/27/css-in-2022)**

- Hotlist - `Cascade Layers`, `Viewport Unit`, `overscroll-behavior`, `Media Query Range` ...

### **[A Deep CSS Dive Into Radial And Conic Gradients](https://www.smashingmagazine.com/2022/01/css-radial-conic-gradient)**

- 방사형과 원뿔형 그래디언트에 대한 개요, 작동 방식, 차이점과 유사점, 사용 사례 등

### **[30 Frontend Tips](https://kittygiraudel.com/2022/01/04/30-frontend-tips/)**

- 보다 나은 프론트 개발자가 되기 위한 조언 30가지

# Node

### **[NAPI-RS 2.0: A Minimal Library for Building Node Addons in Rust](https://napi.rs/blog/announce-v2)**

- 러스트에서 JS값을 정의하기 위한 매크로 API 도입
- Support async fn

### **[fast-json-stringify 3.0: 2x Faster than `JSON.stringify()`?](https://github.com/fastify/fast-json-stringify)**

- fastify팀에서 만든 fast json

# Javascript

### **[Make JS Games: How to Code Games with JavaScript](https://makejsgames.com/)**

- [repl.it](http://repl.it) 에서 Kaboom.js 로 게임 만들기 튜토리얼
- 각 화면을 누르면 해당 게임 제작 튜토리얼(repl docs)로 이동

### **[Eleventy v1.0: The JS-Powered Static Site Generator](https://www.11ty.dev/)**

- 지킬의 대안으로 만들어진 11ty 1.0 릴리즈

### **[Parcel CSS: A New CSS Parser, Compiler, and Minifier Written in Rust](https://parceljs.org/blog/parcel-css/)**

- parcel 2.2 릴리즈. CSS 파서를 러스트로 재작성
- https://github.com/servo/rust-cssparser 를 기반으로 작동

### **[formed The Astro Technology Company](https://astro.build/blog/the-astro-technology-company/)**

- Skypack(pika)이 Astro에 합류하고 $7M을 모집하여 Astro Technology Company 라는 회사 설립

### **[How Storybook Migrated 541 Components From Styled Components to Emotion (Without Bugs)](https://storybook.js.org/blog/541-components-from-styled-components-to-emotion/)**

- 스토리북은 이모션을 사용하고, 크로마틱은 스타일드 컴포넌트를 사용 ⇒ 이모션으로 통합
- 마이그레이션을 위해 커밋 시 이전스냅샷과 이후 스냅샷을 비교, 버그인지 의도인지 파악
- `const Arrow = styled(Icon).attrs({ icon: 'arrowdown' })``;` 과 같이 이모션이 지원하지 않는 코드에 대한 작업

### **[Form Validation with the Constraint Validation API](https://blog.openreplay.com/form-validation-using-javascript-s-constraint-validation-api)**

- Constraint Validation API 를 통한 validateform 소개
- `checkValidity()` , `reportValidity()`

### **[Danfo.js 1.0: Data Analysis Toolkit and Structures](https://github.com/javascriptdata/danfojs)**

- Pandas를 보고 영감받아 js버전으로 제작한 도구