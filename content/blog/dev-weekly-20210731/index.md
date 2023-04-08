---
title: dev-weekly 2021-07-31
date: "2021-07-31T09:00:00.000Z"
description: "dev-weekly 2021-07-31"
tags: ["javascript", "node", "css"]
---

## CSS

### **[Prevent Unwanted Layout Shifts Caused by Scrollbars With the Scrollbar-Gutter CSS Property](https://www.bram.us/2021/07/23/prevent-unwanted-layout-shifts-caused-by-scrollbars-with-the-scrollbar-gutter-css-property)**

- Scrollbar-Gutter 을 사용하면 레이아웃 시프트 없이 overflow: scroll에 대한 대응이 됨 - 스크롤이 생기기 전은 padding으로 잡아줌
- 지금은 flag값을 설정해야 하는 크롬 카나리지만 추후에는 크롬에 지원될 것

### **[Compat 2021 Mid-Year Update: Flex Gap Everywhere](https://web.dev/compat2021-midyear)**

- flexbox gap(safari), grid, position: sticky (thead bug), aspect-ratio, transform(perspective, preserve-3d) 등의 개선

### **[Thinking About The Cut-Out Effect: CSS or SVG?](https://ishadeed.com/article/thinking-about-the-cut-out-effect)**

- CSS, SVG를 통한 잘라내기 효과들
    - SVG Clip Path
    - CSS Mask - radial-gradient
    - SVG mask
- 실제 사용되는 예시들(User Avatar, multi-profile-image, header logo)을 통한 설명

### **[The Large, Small, and Dynamic Viewports](https://www.bram.us/2021/07/08/the-large-small-and-dynamic-viewports)**

- Large viewport, small viewport, dynamic viewport
    - [l, s, d][vh, vw, vmin, vmax]
- [https://www.w3.org/blog/CSS/2021/07/15/css-values-4-viewport-units/](https://www.w3.org/blog/CSS/2021/07/15/css-values-4-viewport-units/)

### **[The Accessibility Stalemate](https://christianheilmann.com/2021/07/20/the-accessibility-stalemate)**

- 해결해야 하는 접근성에 대한 몇 가지 진실/편견
    - 무서움 - 접근성의 베스트 셀링 포인트는 *"모두가 사용할 수 있도록 하면 더 나은 제품을 만들 수 있습니다."* 가 아니라, *"제품에 접근 할 수 없으면 소송당할 것입니다."*
    - 지루함 - 사람들에게 규정을 준수하기 위해 보이지 않는 일을 해야 한다고 표현
    - 복잡함

### **[Moving on a Penrose Triangle](https://codepen.io/amit_sheen/pen/gOWXMJp)**

- CSS only

# Node

### **[ws 8.0: Fast, Stable WebSocket Client and Server for Node](https://github.com/websockets/ws/releases/tag/8.0.0)**

- ws 8.0 릴리즈

### **[Insight: A Module to Help You Understand How Your Tool Is Being Used](https://github.com/yeoman/insight)**

- 메트릭 리포팅하는 도구 GA or Yandex

# Javascript

### **[Node v16.6.0 (Current) Released](https://nodejs.org/en/blog/release/v16.6.0/)**

- v8 9.2 적용 - [Array.prototype.at](http://array.prototype.at) 지원
    - [1, 2, 3].at(-1) // 3

### **[Yarn 3.0: What's New in the Alternative JavaScript Dependency Manager](https://dev.to/arcanis/yarn-3-0-performances-esbuild-better-patches-e07)**

- yarn3 12월부터 작업

### **[How Do Chrome Extensions Impact Browser Performance?](https://www.debugbear.com/blog/chrome-extension-performance-2021)**

- 크롬 확장 프로그램이 브라우저 성능에 미치는 영향
    - CPU, Memory, Rendering Time 등
    - adblock은 요청을 막아서 퍼포먼스에 이로움

### **release**

- [https://github.com/facebookexperimental/Recoil/releases/tag/0.4.0](https://github.com/facebookexperimental/Recoil/releases/tag/0.4.0) 리코일 0.4.0

### **[On WebView2 and Electron](https://www.electronjs.org/blog/webview2)**

- 일렉트론 측에서 작성한, MS의 webview2와 일렉트론 비교한 글

### **[Size Limit 5: A Performance Budgeting Tool for JavaScript](https://github.com/ai/size-limit)**

- ci의 커밋을 확인하고, 최종 결과물의 비용(파일 크기, 렌더링 시간 등)을 계산해서
한도초과하면 풀리퀘에 오류 표시 해주는 도구
- mobx, material-ui, browserlist, postCSS 등등의 도구들이 사용 중

### **[JavaScript Cookie 3.0: A Simple API for Handling Browser Cookies](https://github.com/js-cookie/js-cookie/releases/tag/v3.0.0)**

- JS Cookie 3.0 릴리즈