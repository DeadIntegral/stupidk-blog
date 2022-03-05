---
title: dev-weekly 2022-02-26
date: "2022-02-26T10:30:00.000Z"
description: "dev-weekly 2022-02-26"
tags: ["javascript", "css", "node"]
---

# CSS

### **[CSS Scroll Snap Slide Deck That Supports Live Coding](https://css-tricks.com/css-scroll-snap-slide-deck)**

- JS를 사용하지 않고, CSS 데모를 실시간으로 편집할 수 있는 슬라이드

### **[Repobeats](https://repobeats.axiom.co/)**

- Github readme에 insight section 데이터를 차트로 보여주는 도구

# Node

### **[Caxa: Package Node Apps Into Executable Binaries](https://github.com/leafac/caxa)**

- vercel의 pkg, nexe처럼 single executable 노드 앱을 만드는 도구

# Javascript

### **[What Are Wrapper Objects for JavaScript's Primitive Values?](https://2ality.com/2022/02/wrapper-objects.html)**

```jsx
> 'abc' instanceof String
// false
> new String('abc') instanceof String
// true
```

- primitive value는 연결된 래퍼 클래스의 인스턴스와 다름

### **[How to Read the ECMAScript Specification](https://timothygu.me/es-howto/)**

- ECMA spec과 유사하게 작성한 문서
- JS가 처음인 사람에겐 권장하지 않음

### **[Cheerp 2.7: Compile C++ to WebAssembly and JavaScript](https://medium.com/leaningtech/cheerp-2-7-compile-cpp-to-webassembly-plus-javascript-c9b3ef7e318b)**

- Cpp코드를 WASM과 JS로 컴파일 하는 도구 Cheerp 2.7 릴리즈
- Cheerp는 LLVM clang의 오픈 소스 포크
- Emscription 3.1.5 와의 벤치마크 결과

### **[How to Reliably Send an HTTP Request on Leaving a Page](https://css-tricks.com/send-an-http-request-on-page-exit/)**

- 페이지 이동과 함께 http request를 하면 이동이 먼저 완료됐을 때 요청 취소
- 요청이 완료될 때 까지 기다렸다가 전환할 수 있지만 좋지 않은 UX
- `keepalive` 플래그를 사용하는 방법
- `Navigator.sendBeacon()` 을 사용하는 방법 - low priority