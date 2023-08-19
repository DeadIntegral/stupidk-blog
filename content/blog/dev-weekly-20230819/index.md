---
title: dev-weekly 2023-08-19
date: "2023-08-19T17:35:00.000Z"
description: "dev-weekly 2023-08-19"
tags: ["javascript", "node", "css"]
---

# CSS

### **[Four new CSS features for smooth entry and exit animations](https://developer.chrome.com/blog/entry-exit-animations/)**

- keyframe에서 display, content-visibility 를 지원 (크롬 116)
    - ex) `@keyframes fade-out { 100% { opacity: 0; display: none; } }` 를 주면 애니메이션이 끝나고 display: none이 적용.
- `transition-behavior`. transition이 끝나고 display가 적용되도록 지원
    - 축약 가능
        
        ```css
        .card {
          transition: opacity 0.5s, display 0.5s allow-discrete;
        }
        
        .card.fade-out {
          opacity: 0;
          display: none;
        }
        ```
        
- `@starting-style` rule
    - `@starting-style { .item { opacity: 0; height: 0; } }`
- `overlay` 프로퍼티
    - dialog나 popover 트랜지션에 overlay를 넣으면 애니메이션을 적용할 때 오버레이가 최상위 레이어에 유지되도록 작동.

### **[The new @font-face syntax](https://fullystacked.net/posts/new-font-face-syntax)**

- 사파리17, 파이어폭스 106, 크롬 108 부터 새로운 font-face 문법 제공
    
    ```css
    @font-face {
    	font-family: "source sans";
    	/* AS-IS */
    	src: url("SourceSansVariable.woff2") format("woff2-variations");
    
    	/* TO-BE */
    	src: url("SourceSansVariable.woff2") format(woff2) tech(variations);
    }
    ```
    

# Node

### **[Fresh 1.4 – Faster Page Loads, Layouts and More](https://deno.com/blog/fresh-1.4)**

- 사전 컴파일로 성능 향상
    - 빌드 없이 빠른 배포를 유지해왔지만, 큰 island의 경우 JIT가 눈에 띄게 느리다는 것을 인지하여 배포 시간에 영향을 덜 주면서 사전 컴파일 하도룩 변경
- 서버에서 직접 html, head 등의 태그를 사용 가능하도록 수정
- 디렉토리 스코프를 가진 _layout.tsx 기능 지원. (넥스트13과 같은 기능) 상속 해제도 가능.

# Javascript

### **[How we reduced the size of our JavaScript bundles by 33%](https://dropbox.tech/frontend/how-we-reduced-the-size-of-our-javascript-bundles-by-33-percent)**

- dropbox에서 모듈 번들러를 rollup으로 변경하고 tree shaking을 조절하여 번들 개선한 후기

### **[Discover threejs](https://discoverthreejs.com/)**

- threejs 코어 개발자 중 한명이 제공하는 가이드 (무료 책)

### **[Tagger: Zero Dependency, Vanilla JavaScript Tag Editor](https://github.com/jcubic/tagger)**

- 의존성 없는 tag 에디터

### Release

- [jest-dom 6.0](https://deno.com/blog/fresh-1.4)
- [electron 26.0](https://www.electronjs.org/blog/electron-26-0) - chrome 116
- [angular 16.2](https://github.com/angular/angular/releases/tag/16.2.0)
- [playwright 1.37](https://github.com/microsoft/playwright/releases/tag/v1.37.0)
- [svgr 8.1](https://github.com/gregberge/svgr/releases/tag/v8.1.0)
- [preact 10.17.0](https://github.com/preactjs/preact/releases/tag/10.17.0)

# ETC

### **[What's New in DevTools (Chrome 117)](https://developer.chrome.com/blog/new-in-devtools-117/)**

- 네트워크 패널
    - 응답 콘텐츠 재정의 지원
    - 크롬 익스텐션 숨기기 지원
    - HTTP status code 옆에 사람이 읽을 수 있는 문구 추가
- 소스 패널에서 코드 folding 기능 제공
- 써드파티 쿠키 차단 모의 기능