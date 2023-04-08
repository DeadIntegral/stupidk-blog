---
title: dev-weekly 2021-12-18
date: "2021-12-18T11:00:00.000Z"
description: "dev-weekly 2021-12-18"
tags: ["css", "node", "javascript"]
---

# CSS

### **[Discover the State of CSS 2021 Survey Results](https://2021.stateofcss.com/ko-KR/)**

- State of CSS 2021 Result

### **[Standardizing Focus Styles With CSS Custom Properties](https://css-tricks.com/standardizing-focus-styles-with-css-custom-properties/)**

- 크롬과 파이어폭스에서 outline은 이제 border-radius를 따름

### **[Building a Toast Component](https://web.dev/building-a-toast-component)**

- `<output>` , `role=status`, `prefers-color-scheme`, `prefers-reduced-motion: no-preference` 등으로 접근성 향상시킨 토스트

# Node

### **[Node's New(ish) `node:` Protocol Imports](https://2ality.com/2021/12/node-protocol-imports.html)**

- **`import** * **as** fs **from** 'node:fs/promises';`
- 내장 모듈을 가져왔다는것을 명시할 수 있음
- [https://gist.github.com/sindresorhus/a39789f98801d908bbc7ff3ecc99d99c](https://gist.github.com/sindresorhus/a39789f98801d908bbc7ff3ecc99d99c)

### **[Deno joins TC39](https://deno.com/blog/deno-joins-tc39)**

- 서버 측 JS 유저에게 도움이 되는 기능과 언어 개선을 추진하기 위해서

### **[Got 12.0: A Powerful HTTP Request Library for Node](https://github.com/sindresorhus/got/releases)**

- TS 이용자의 경우 TS 4.6 이전까지는 Got11 이용
- node에서 http2 비활성화 하는데, got13에선 디폴트로 활성화 가능하도록 할 것

# Javascript

### **[Deep-Copying in JavaScript Using `structuredClone`](https://web.dev/structured-clone/)**

- Node17, Deno 1.14, 각 브라우저의 나이틀리 버전에서 제공
- `JSON.stringify` 에서는 `Map`, `Set`, `Date`, `RegExp`, `ArrayBuffer` 가 들어있으면 오작동
- 단 프로토타입 체인, 함수는 폐기

### **[A Recap of React Conf 2021](https://reactjs.org/blog/2021/12/17/react-conf-2021-recap.html)**

- React 18 and concurrent features
- React 18 for Application Developers
- Streaming Server Rendering with Suspense

### **[Create React App 5.0: The Popular 'One Command' React App Builder](https://github.com/facebook/create-react-app/releases/tag/v5.0.0)**

- Webpack5, Jest27, ESLint 8, Tailwind 지원
- Fast Refresh 향상 및 버그 수정
- 노드10, 12 지원 종료

### **[quick-lint-js 1.0: An Alternative to ESLint](https://quick-lint-js.com/blog/version-1.0/)**

- ESLint, Flow, TypeScript 보다 110배 빠른 성능
- VSCode, EMacs, Vim, NeoVim 플러그인 제공
- ESLint보다 나은 에러 리포트