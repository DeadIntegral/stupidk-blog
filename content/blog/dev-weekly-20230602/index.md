---
title: dev-weekly 2023-06-02
date: "2023-06-02T23:50:00.000Z"
description: "dev-weekly 2023-06-02"
tags: ["javascript", "css", "node", "etc"]
---

# CSS

### **[Toaster](https://petertyliu.github.io/toaster/)**

- pure CSS, HTML로 만든 3D 에디터.
- WebGL도 Canvas도 사용하지 않음.

### **[SupportsCSS](https://supportscss.dev/)**

- Modernizr처럼 사용자의 브라우저에서 CSS Support를 평가
- `@supports` 는 container, layer와 같은 at-rules 들을 평가 불가. 이 도구는 가능.

# Node

### **[Advanced Fastify: Hooks, Middleware, and Decorators](https://blog.appsignal.com/2023/05/24/advanced-fastify-hooks-middleware-and-decorators.html)**

- Fastify 시리즈. fastify에서 hook, 미들웨어, 데코레이터를 사용하는 기본적인 방법 및 예제를 통한 설명
- Fastify의 데이터 검증 - JSON 스키마

### **[color-names: Large list of handpicked color names](https://github.com/meodai/color-names)**

- 매우 큰 색상 이름 목록. 글 작성 시점엔 30126개의 색상에 이름 부여.

### **[got: Human-friendly and powerful HTTP request library for Node.js](https://github.com/sindresorhus/got/releases/tag/v13.0.0)**

- got 13 릴리즈. node 16 필요.
- enableUnixSocket 옵션 기본값 false로 변경 - 대부분의 유저는 필요하지 않음.

# Javascript

### **[300ms Faster: Reducing Wikipedia's Total Blocking Time](https://www.nray.dev/blog/300ms-faster-reducing-wikipedias-total-blocking-time/)**

- Wikipedia의 TBT(Total Block Time) 개선기.
    - TBT는 FCP와 TTI 사이의 값. 각 렌더링 사이의 50ms가 넘는 지연의 합산.
- 프로파일링 결과 jQuery on 에서 블록킹. 이 부분을 개선.

### **[WEB SHARE API IS A W3C RECOMMENDATION](https://www.w3.org/blog/news/archives/9931)**

- Web Share API 가 이제 W3C 권장.
- 공유 가능 대상은 user agent에서 제공.

### **[JavaScript Macros in Bun](https://bun.sh/blog/bun-macros)**

- Bun의 새 기능 매크로 - 번들 타임에 JS 함수를 하는 매커니즘

### **[Sharing WebSocket Connections between Browser Tabs and Windows](https://brightinventions.pl/blog/sharing-websocket-connections-between-browser-tabs-and-windows/)**

- 사용자가 탭, 창을 켤 때 마다 소켓연결을 하면 부담. shared worker를 사용하여 단일 연결 하기.
- shared worker 생성하기, 메모리 관리하기 등 기본적인 예제.

### **Release**

- [Electron 25.0.0](https://www.electronjs.org/blog/electron-25-0)
- [Bootstrap 5.3.0](https://blog.getbootstrap.com/2023/05/30/bootstrap-5-3-0/)
- [Parcel 2.9](https://parceljs.org/blog/v2-9-0/)

# ETC

### **[Safari allows to configure password autofilling](https://www.stefanjudis.com/today-i-learned/safari-allows-to-configure-password-autofilling/)**

- safari는 다음과 같은 passwordrules 프로퍼티 제공.
    - `<input type="password" passwordrules="minlength: 8; required: lower; required: upper; required: digit; required: [_];">`

### **[Announcing WASIX](https://wasmer.io/posts/announcing-wasix)**

- WASM ABI 를 개선하고 POSIX와의 호환성을 높인 결과물 WASIX 출시
- WASIX란 애플리케이션을 지금 컴파일 하고 사용할 수 있도록 해주는 시스템 콜 확장.