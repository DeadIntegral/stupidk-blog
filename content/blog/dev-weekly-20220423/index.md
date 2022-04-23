---
title: dev-weekly 2022-04-23
date: "2022-04-23T09:00:00.000Z"
description: "dev-weekly 2022-04-23"
tags: ["javascript", "css", "node"]
---

# CSS

### **[Picture Perfect Images With the Modern  Element](https://stackoverflow.blog/2022/03/28/picture-perfect-images-with-the-modern-element)**

- img 태그의 중요성 설명 및 Web Vitals에 대한 영향
- CLS, LCP, Responsive, DPR, format 등 다양한 개념과 최적화 하기
- preload와 lazy로딩, First Input Delay

### **[Forced Colors Explained: A Practical Guide](https://polypane.app/blog/forced-colors-explained-a-practical-guide)**

- 고대비 모드(High contrast mode)에 대한 설명
- `@media (forced-colors: active)`
- 사이트를 외관을 좋게 만드는게 아니라, 고객의 희망 사항을 존중하도록 만드는 것

### **[Childish Font Sizes](https://cloudfour.com/thinks/childish-font-sizes)**

- 과거 10 픽셀에서 한동안 모든 주요 브라우저의 기본값은 16픽셀. 이제는 더 키우자는 글
- 글자가 커질 때 얻을 수 있는 장점들

# Node

### **[Node.js 18 (Current) Released](https://nodeweekly.com/link/122584/154188e1e3)**

- V8 10.1 업데이트, fetch API(실험), core test runner module(실험)
- 빌드 시점에 사용자 영역 스냅샷(실험)

### **[chalk-animation: Colorful Animations in Terminal Output](https://github.com/bokub/chalk-animation)**

- 터미널 스타일링 도구 chalk로 만든 터미널 애니메이션

### release

- [https://github.com/google/zx/releases/tag/6.1.0](https://github.com/google/zx/releases/tag/6.1.0)
- [https://github.com/googleapis/google-auth-library-nodejs/releases/tag/v8.0.0](https://github.com/googleapis/google-auth-library-nodejs/releases/tag/v8.0.0)

# Javascript

### **[Lexical: An Extensible Text Editor Library (That Does Things Differently)](https://javascriptweekly.com/link/122666/4e4af8cb63)**

- 메타(페이스북)의 새 에디터. draftjs 대신 사용할 프레임워크
- 렉시컬 노드 트리가 존재하고, 노드 변경이나 커맨드 listen 가능
- 크로미움 엣지+, 사파리11+ 브라우저 지원

### **[Ember 4.3 Released](https://blog.emberjs.com/ember-released-4-3/)**

- 사용해야 하는 이유: [https://whyember.com/](https://whyember.com/)

### In brief

- **[GitHub profile private](https://github.blog/changelog/2022-04-21-private-profiles/)** - 깃헙 프로필 비공개 가능
- **[JavaScript for MS-DOS](https://hackaday.com/2022/04/15/javascript-is-everywhere-even-msdos/)**
    - dos 및 관련 운영체제용 js 엔진 [jsh](https://github.com/SuperIlu/jSH)
    - 최소사양: 하드웨어 80386 4MB, 램 8MB 이상
- **[WebAssembly 2.0](https://www.w3.org/TR/wasm-core-2/)** - 첫 public working draft

### Release

- [https://deno.com/blog/v1.21](https://deno.com/blog/v1.21)
- [https://github.com/reduxjs/react-redux/releases/tag/v8.0.0](https://github.com/reduxjs/react-redux/releases/tag/v8.0.0)
- [https://github.com/neutralinojs/neutralinojs/releases/tag/v4.5.0](https://github.com/neutralinojs/neutralinojs/releases/tag/v4.5.0)
- [https://github.com/fastify/fast-json-stringify/releases/tag/v3.1.0](https://github.com/fastify/fast-json-stringify/releases/tag/v3.1.0)

### **[V8's Faster Initialization of Instances with New Class Features](https://v8.dev/blog/faster-class-features)**

- V8엔진에서 js class의 field, private method 초기화 성능 향상 (노드18에 적용)

### **[A Quick Guide to Mitosis: Why You Need It and How You Can Use It](https://www.builder.io/blog/mitosis-a-quick-guide)**

- 컴파일 타임 프레임워크 - 각 프레임워크 컴포넌트 생성기
- Vue, React, Angular, Svelte, RN, Swift, SolidJS, Stencil, WebComponent... 등 지원