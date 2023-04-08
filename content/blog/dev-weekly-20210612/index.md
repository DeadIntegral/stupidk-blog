---
title: dev-weekly 2021-06-12
date: "2021-06-12T08:30:00.000Z"
description: "dev-weekly 2021-06-12"
tags: ["javascript", "node"]
---

# Node

### **[Introducing libSquoosh: Experimental Image Optimization from Node](https://web.dev/introducing-libsquoosh/)**

- Squoosh CLI가 빌드 된 실험적인 노드 라이브러리
- Squoosh.app 브라우저에서 이미지를 압축하는 PWA (WASM)

### **[PM2 5.0 Released: The Production Process Manager](https://github.com/Unitech/pm2/blob/master/CHANGELOG.md#500)**

- PM2 5.0 릴리즈
- System Monitoring - 중요한 서버 메트릭들 모니터링 (온오프 가능)

### **[Mocha 9.0 Released: The Popular JavaScript Test Framework](https://github.com/mochajs/mocha/releases/tag/v9.0.0)**

- Node 10.x 지원 중단
- 디폴트 셋팅이 CommonJS 에서 ESM 으로 이동

## Go

### **[Go 1.17 Beta 1 Released](https://groups.google.com/g/golang-announce/c/i4EliPDV9Ok/m/MxA-nj53AAAJ)**

- lazy module loading

# Javascript

### **[Introducing Astro: Ship (Even) Less JavaScript](https://astro.build/blog/introducing-astro)**

- 더 많은 js는 반대 방향, 더 적게 작성할 수 있는 정적 사이트 빌더 Astro 소개
- 최종 빌드에서 JS를 모두 제거, 100% 정적 HTML
- 캐러셀과 같이 JS가 필수로 필요한 컴포넌트에서는 해당 컴포넌트(와 종속성)만 로드
- islands architecture
- 느린 사이트 구축을 어렵게 만드는 도구
- [https://github.com/snowpackjs/astro#-guides](https://github.com/snowpackjs/astro#-guides)

### **[The Plan for React 18](https://reactjs.org/blog/2021/06/08/the-plan-for-react-18.html)**

- 컨커런트 모드를 충돌없이 마이그레이션 가능하도록 설계(페이스북의 수만개 컴포넌트가 충돌없음)

### **[Introducing Chrome's New Memory Inspector](https://developer.chrome.com/blog/memory-inspector/)**

- 크롬 91에 추가된 메모리 inspector
    - ArrayBuffer, TypedArray, DataView, Wasm
- HxD와 같은 UI를 가진 패널을 보여줌 - 메모리 버퍼 옆에 아스키 값을 같이 표시
    - 사용자가 endian을 직접 선택 가능
- 설계목표 - 버퍼 크기에 독립적인 성능 및 메모리 사용

### **[Vue.js 3.1.0 (Pluto) Released](https://github.com/vuejs/vue-next/releases/tag/v3.1.0)**

- vue2에서 vue3로 마이그레이션하는 도구를 제공
- 성능향상, 디프리케이션, 브레이킹 체인지, 버그픽스들

## Quick Bits

### **[https://code.visualstudio.com/updates/v1_57](https://code.visualstudio.com/updates/v1_57)**

- VSCode 업데이트
- JS디버거가 Edge Devtools와 통합되어 DOM, Style, Network inspector 제공

### **[https://developer.chrome.com/en/blog/crx-scripting-api/](https://developer.chrome.com/en/blog/crx-scripting-api/)**

- chrome.scripting API - 크롬 익스텐션 개발에 사용하는 새 API(보안 강화)

### **[https://playwright.dev/docs/next/trace-viewer/](https://playwright.dev/docs/next/trace-viewer/)**

- playwright trace를 도와주는 GUI 도구
- [https://github.com/microsoft/playwright/releases/tag/v1.12.0](https://github.com/microsoft/playwright/releases/tag/v1.12.0)