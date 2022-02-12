---
title: dev-weekly 2022-02-12
date: "2022-02-12T08:30:00.000Z"
description: "dev-weekly 2022-02-12"
tags: ["javascript", "node"]
---

# Node

### **[Pintora: An Extensible Text-to-Diagram Rendering Library](https://github.com/hikerpig/pintora)**

- mermaid.js와 유사한 프로그램
- 브라우저에서는 SVG, Canvas 지원, nodejs에서는 PNG,JPG,SVG file 지원

### [Google Cloud Move **Node.js 10 to Maintenance**](https://cloud.google.com/blog/products/application-development/google-cloud-sdk-moves-nodejs-10-to-maintenance-mode)

- 구글 클라우드는 노드10 지원을 유지보수 모드로 낮춤

### **[Spectron: Deprecation Announcement](https://github.com/electron-userland/spectron/issues/1045)**

- 일렉트론 테스팅 도구 Spectron Deprecate

### **[remix-electron: An Initial Electron Integration for Remix](https://github.com/itsMapleLeaf/remix-electron)**

- 브라우저에서 실행되지 않는 일렉트론 API도 사용 가능한 노드 프로세스

### **[zx 5.0: A Tool for Writing Better Shell Scripts](https://github.com/google/zx/releases/tag/5.0.0)**

- js로 쉘스크립트 만드는 도구 zx 5.0 릴리즈 - YAML 패키지 추가
- commonJS 지원 중단, ts는 `node --loader ts-node/esm script.ts` 형태로 사용할 것

# Javascript

### **[Apache ECharts 5.3: Open Source JS Visualization Library](https://echarts.apache.org/handbook/en/basics/release-note/5-3-0/)**

- ECharts 5.3릴리즈 애니메이션, 렌더링 성능 향상, 서버사이드 렌더링
- Pie Chart 레이아웃 최적화
- Bar Chart 대형모드(데이터 > 2Kb) 최적화

### **[Move Over JavaScript? How Some Backend Languages are Coming to the Front-End](https://javascriptweekly.com/link/119706/4e4af8cb63)**

- liveviews 라는 새로운 도구 ⇒ 모든 UI 요소는 서버에서 렌더링해서 웹소켓으로 전송, 클라이언트는 HTML, CSS를 수신해서 표시
- 클라이언트CPU와 배터리에 가해지는 부담

### **[WebGL 2.0 is now broadly supported](https://www.khronos.org/blog/webgl-2-achieves-pervasive-support-from-all-major-web-browsers)**

- iOS 15에서 WebGL 2.0을 지원하면서 모든 메이저 브라우저가 WebGL 2.0 지원
- `const gl = document.getElementById('myCanvas').getContext('webgl2');`

### Release

- vite 2.8.0
    - [https://github.com/vitejs/vite/blob/main/packages/vite/CHANGELOG.md#280-2022-02-09](https://github.com/vitejs/vite/blob/main/packages/vite/CHANGELOG.md#280-2022-02-09)
    - publish size, install size 35%감소
- vue 3.0 default
    - [https://blog.vuejs.org/posts/vue-3-as-the-new-default.html](https://blog.vuejs.org/posts/vue-3-as-the-new-default.html)

### **[How the Angular Compiler Works](https://blog.angular.io/how-the-angular-compiler-works-42111f9d2549)**

- ngc의 컴파일 과정에 대해 설명해주는 포스트
- 타입스크립트와 앵귤러 모두에서 `incremental` 컴파일 모드 제공

### **[Griffel: CSS-in-JS with Ahead-of-Time Compilation](https://github.com/microsoft/griffel)**

- MS 에서 만든 CSS in JS 도구
- zero에 근접한 런타임, JS객체로 정의한 SSR 지원

### **[Fable 3.7: A Mature F# to JavaScript Compiler](https://github.com/fable-compiler/Fable/releases/tag/3.7.0)**

- F#을 JS 에코시스템으로 가져오는 컴파일러 Fable 3.7 릴리즈
- [https://fable.io/samples-browser/](https://fable.io/samples-browser/)