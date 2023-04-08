---
title: dev-weekly 2021-08-14
date: "2021-08-14T09:00:00.000Z"
description: "dev-weekly 2021-08-14"
tags: ["javascript", "node", "css"]
---

# CSS

### **[Using CSS Shapes for Interesting User Controls and Navigation](https://css-tricks.com/using-css-shapes-for-interesting-user-controls-and-navigation)**

- `shape-outside` 를 통해 이미지를 따른 UI 작업
    - 배경이 투명한 이미지만 가능

### **[CSS Nesting, Specificity and You](https://kilianvalkhof.com/2021/css-html/css-nesting-specificity-and-you)**

- CSS Nesting이 곧 브라우저에 도입
- `:is` 에 대한 설명(현재 ie를 제외한 모던 브라우저는 전부 지원)

### **[Using HSL Colors In CSS](https://www.smashingmagazine.com/2021/07/hsl-colors-css)**

- HSL에 대한 쉬운 설명

### **[A Deep Dive on Skipping to Content](https://css-tricks.com/a-deep-dive-on-skipping-to-content)**

- 컨텐츠 스킵 기술에 대한 설명
    - landmarks
    - skip links
    - 예제를 위한 몇가지 웹 사이트
- 웹접근성

### **[Useful and Useless Code Comments](https://blog.jim-nielsen.com/2021/useful-and-usless-code-comments)**

- 주석이 코드를 똑같이 되풀이할 때 그런 주석은 필요 없다는 입장에 대한 설명
- 그 주석이 누구에게 쓸모 없는것인지 자문하기. 해당 코드가 낯선사람에게는 도움이 될 수 있음

### **[Pure CSS Cube Cannon](https://codepen.io/amit_sheen/pen/BaRqKJb)**

- only CSS, HTML 로 만들어진 큐브 캐논.
- 관점변경 버튼, 앵글 조절 버튼, 슛, 리로드 등의 버튼(css로 제어)

## Node

### **[Deno 1.13 Released](https://deno.com/blog/v1.13)**

- V8 9.3
- 네이티브 HTTP 서버 API 안정화
- TLS에 시스템 인증서 지원 및 비활성화 기능

### **[V8 Release v9.3](https://v8.dev/blog/v8-release-93)**

- Sparkplug batch compilation
    - 전체 컴파일 타임(ignition + Sparkplug)을 최대 44% 단축
- Object.hasOwn
    - Object.prototype.hasOwnProperty.call 에 대한 별칭
    - `Object.hasOwn({ prop: 42 }, 'prop')` // true
- 안드로이드에서 신뢰할 수 없는 코드 완화 비활성화

# Javascript

### **[Vue 3.2 Released](https://blog.vuejs.org/posts/vue-3.2.html)**

- 뷰 3.2 릴리즈

### **[Next.js 11.1 Released](https://nextjs.org/blog/next-11-1)**

- 보안 업데이트
- ES 모듈 서포트
- Rust-based Tooling - SWC 통합
- Faster Data Fetching - HTTP `keep-alive`를 통한 프리렌더링 성능 향상
- 소스맵 사용 중 성능 향상(메모리 감소, 빌드 속도 증가)
- 린트 향상
- `next/image` 향상

### **[https://devblogs.microsoft.com/typescript/announcing-typescript-4-4-rc/](https://devblogs.microsoft.com/typescript/announcing-typescript-4-4-rc/)**

- TS 4.4 RC

### **[Improving Responsiveness in Text Inputs](https://nolanlawson.com/2021/08/08/improving-responsiveness-in-text-inputs/)**

- input 입력 처리 디바운싱 대신 `requestIdleCallback` 사용해보기

### **[JSZip: Create, Read and Edit .zip Archive Files](https://stuk.github.io/jszip/)**

- 모든 메이저 브라우저에서 작동하는 JS zip
- [https://github.com/Stuk/jszip](https://github.com/Stuk/jszip)

### **[styled-jsx 4.0: Full CSS Support for JSX Without Compromises](https://github.com/vercel/styled-jsx)**

- vercel의 스타일드 jsx 4.0 릴리즈

### **[Hora: Efficient Approximate Nearest Neighbor Search Algorithms](https://github.com/hora-search/hora)**

- 러스트로 작성 된 nearest neighbor 검색 알고리즘 (WASM 사용 가능)