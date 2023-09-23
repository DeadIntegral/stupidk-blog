---
title: dev-weekly 2023-09-23
date: "2023-09-23T10:45:00.000Z"
description: "dev-weekly 2023-09-23"
tags: ["javascript", "node", "css"]
---

# CSS

### **[Solved by CSS Scroll-Driven Animations: Detect if an element can scroll or not](https://www.bram.us/2023/09/16/solved-by-css-scroll-driven-animations-detect-if-an-element-can-scroll-or-not/)**

- CSS로 스크롤 가능한지 여부 확인하여 콘텐츠 인디케이터 만들기
- CSS 변수를 선언하고 scroll 에 애니메이션 바인드. keyframe에서 애니메이션이 끝나면 변수값 변경
    
    ```css
    .container {
    	...
      --can-scroll: 0;
      animation: detect-scroll;
      animation-timeline: scroll(self);
    }
    
    @keyframes detect-scroll {
      from, to  {
        --can-scroll: 1;
      }
    }
    ```
    

# Node

### **[Node.js Have a mascot](https://github.com/nodejs/admin/issues/828)**

- nodejs 비공식 마스코트 v8 미사일에 탄 거북이.

### **[My thoughts on Bun and other Adventures](https://adventures.nodeland.dev/archive/my-thoughts-on-bun/)**

- fastify 창시자의 Bun에 대한 생각
    - bun 1.0 이 fastify 지원 안한다고 하자 bun 1.0.2에서 지원
        - [https://bun.sh/blog/bun-v1.0.2#bugfix-for-fastify](https://bun.sh/blog/bun-v1.0.2#bugfix-for-fastify)

### **[Deno 1.37: Modern JavaScript in Jupyter Notebooks](https://deno.com/blog/v1.37)**

- Deno 1.37에서 주피터 노트북 지원
    - 노트북에서 바로 npm 모듈에 접근 가능
    - ex) npm에서 d3를 가져와서 노트북에 시각화
- VSCode 익스텐션, 언어 서버 지원 추가
- 테스트 개선 - 속도, TAP 리포터
- Node.js 호환성 개선
- 성능개선 - WebAPI 최적화, lockfile v3 업데이트

# Javascript

### **[WebKit Features in Safari 17.0](https://webkit.org/blog/14445/webkit-features-in-safari-17-0/)**

- input search 지원, popover 지원 추가
- font-size-adjust, display: contents, image-set 지원
- Storage API 지원, offscreen canvas에 WebGL 추가(3D도 지원)
- URL.canParse, URLSearchParams has(), delete() 지원
- JPEG XL, AV1 지원
- macOS sonoma를 통해 Web App 지원. (웹사이트 Dock에 추가해서 사용)

### **[free-for.dev](https://free-for.dev/#/)**

- 개발자를 위한 무료 호스팅 서비스 모음. 최근 업데이트.
- 메이저 클라우드의 프리 티어들
- 카테고리별 무료 호스팅 서비스와 제한량 소개

### **[Scaffolding your Chrome extension! Boilerplates](https://github.com/guocaoyi/create-chrome-ext)**

- 크롬 익스텐션 셋팅해주는 도구

### **[Patterns for Reactivity with Modern Vanilla JavaScript](https://frontendmasters.com/blog/vanilla-javascript-reactivity/)**

- PubSub 패턴, CustomEvent, addEventListener를 이용한 방법, Observer 패턴, new Proxy 를 사용하는 방법
- 리액티브 시스템 소개
    - React hooks, Solid signals, Rxjs Observables 등

### **[JS minification benchmarks](https://github.com/privatenumber/minification-benchmarks)**

- JS minify 벤치마크 레포.
- babel-minify, bun, esbuild, swc, tdewolff/minify, terser, uglify-js 등 비교

### **[Next.js 13.5](https://nextjs.org/blog/next-13-5)**

- 성능 향상
    - 로컬 서버 스타트 22%, HMR 29%, 메모리 사용량 40% 감소
- 인기있는 라이브러리 임포트 할 경우 빠른 업데이트
- next/image 향상

### **Release**

- [Remix v2](https://remix.run/blog/remix-v2)
- [Ember.js 5.3](https://github.com/emberjs/ember.js/releases/tag/v5.3.0)

# ETC

### **[Linux kernel map](https://makelinux.github.io/kernel/map/)**

- 리눅스 커널의 구조를 기능, 레이어 별로 시각화한 자료
- 시각화된 자료 내에서 단어를 선택하면 리눅스에서 설명하는 해당 링크로 이동
- 레이어 - user space interface, virtual, bridges, logical, device control, hardware interface
- 기능 - human interface, system, processing, memory, storage, networking

### External

- [모든 서브도메인 찾기](https://news.hada.io/topic?id=10908)