---
title: dev-weekly 2023-08-12
date: "2023-08-12T11:30:00.000Z"
description: "dev-weekly 2023-08-12"
tags: ["javascript", "node"]
---
# Node

### **[Deno 1.36: More flexible security and expanded testing APIs](https://deno.com/blog/v1.36)**

- node20 의 test 사용가능
- deno 벤치마크 기능 향상 - V8의 최적화로 인해 잘못된 벤치를 해결하기 위해 warmup도입
- npm 호환성 개선 등

### **[The easiest way to get started with Electron](https://www.electronjs.org/fiddle)**

- 일렉트론 앱 플레이그라운드 프로그램. github gist에 업로드 가능하고, 다른 사람의 gist도 실행 가능

# Javascript

### **[Blogged Answers: My Experience Modernizing Packages to ESM](https://blog.isquaredsoftware.com/2023/08/esm-modernization-lessons/)**

- redux패키지들을 esm으로 변환한 후기
- 패키지 구성 변경, test도구 변경(vitest), TS호환, 빌드 도구 변경, webpack4지원, nextjs의 서버컴포넌트 이슈 등 다양한 호환성 처리에 대한 후기

### **[Optimizing speed on eBay.com](https://medium.com/@addyosmani/shopping-for-speed-on-ebay-com-6229711d7573)**

- eBay 사이트 최적화
- 스크롤없이 볼 수 있는 영역을 제외한 나머지는 레이지 로드
- 이미지 최적화 - 검색 결과에 나오는 모든 이미지 WebP로 변경
- 인기 검색 결과 프리페치 - 사용자가 검색 결과 상위 10개 항목으로 이동할 가능성이 높다고 가정, 이에 대해 프리페치
- 로그인하지 않은 사용자에 대해서는 에지 네트워크에 캐싱

### **[Bringing Sharp to WebAssembly and WebContainers](https://blog.stackblitz.com/posts/bringing-sharp-to-wasm-and-webcontainers/)**

- WebContainer에 Sharp 추가
- Sharp를 WASM으로 포팅할 때 겪었던 문제와 프로세스
- 샤프는 내부적으로 libvips를 사용. wasm-vips에 편승하여 단일 WASM 모듈로 컴파일 가능하도록 기여
- WebWorker는 동기식으로 생성되지 않고 다음 이벤트 루프 틱에서 생성되도록 예약. 이 비동기를 동기가 가능하도록 emscripten에 기여

### **[Node.js's Config Hell Problem](https://deno.com/blog/node-config-hell)**

- Nodejs에서 수많은 config파일이 생기는 이슈
- deno는 스마트한 기본값을 갖춘 런타임이라 구성이 적게 필요. 프로그래밍은 복잡성 관리에 관한 것.

# ETC

### **[An update on Chrome Security updates – shipping security fixes to you faster](https://security.googleblog.com/2023/08/an-update-on-chrome-security-updates.html)**

- 크롬 116부터 매주 stable channel update 제공.
- 4주 마다 릴리스는 유지하지만, 보안 및 버그수정 업데이트 제공.

### **[What's New in WebGPU (Chrome 116)](https://developer.chrome.com/blog/new-in-webgpu-116/)**

- 웹 코덱 인터그레이션 - HTMLVideoElement에서 external texture 객체를 생성하는 API를 노출

### **[What Does It Mean for Web Browsers to Have a Baseline](https://thenewstack.io/what-does-it-mean-for-web-browsers-to-have-a-baseline/)**

- baseline이란 WebDX Community Group의 프로젝트로 모든 주요 브라우저에서 사용할 수 있는 기능 집합
    - 기준은 크롬, 엣지, 파이어폭스, 사파리의 현재 및 이전버전에서 지원하는 기술
- baseline은 [web.dev](http://web.dev) 뿐 아니라 MDN과 caniuse에도 추가할 것.

### Release

- [puppeteer v21.0](https://github.com/puppeteer/puppeteer/releases/tag/puppeteer-v21.0.0)
- [marked v7.0](https://github.com/markedjs/marked/releases/tag/v7.0.0)
- [Announcing TypeScript 5.2 RC](https://devblogs.microsoft.com/typescript/announcing-typescript-5-2-rc/)
- [esbuild v0.19.0](https://github.com/evanw/esbuild/blob/main/CHANGELOG.md#0190)
- [astro v2.1, Astro 3.0 beta](https://astro.build/blog/astro-2100/)