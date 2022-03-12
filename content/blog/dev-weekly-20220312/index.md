---
title: dev-weekly 2022-03-12
date: "2022-03-12T14:00:00.000Z"
description: "dev-weekly 2022-03-12"
tags: ["javascript", "css", "node"]
---

# CSS

### **[Say Hello to selectmenu, a Fully Style-able select Element](https://css-tricks.com/the-selectmenu-element)**

- OpenUI 그룹에서 제안한 `selectmenu` element 크롬, 엣지 카나리 버전에서 작업 중
- `selectmenu` 는 select의 markup 과 모든 스타일을 변경 가능

### **[Building Web Layouts For Dual-Screen And Foldable Devices](https://www.smashingmagazine.com/2022/03/building-web-layouts-dual-screen-foldable-devices)**

- dual screen 지원을 위한 `horizontal-viewport-segments` media query
- 수평 접기 지원을 위한 `vertical-viewport-segments` media query
- js에서 제어를 위한 `window.visualViewport.segments` API
- [https://web.dev/learn/design/screen-configurations/](https://web.dev/learn/design/screen-configurations/)

### **[Ken Kaneki (Pure CSS)](https://codepen.io/idrinkcss/pen/gOXqvWq)**

- HTML 과 CSS 로 그린 일러스트레이션

# Node

### **[PSD: A Zero-Dependency PSD (Photoshop) Parser for Browser and Node.js](https://webtoon.github.io/psd/)**

- 의존성 없고 웹고 노드에서 사용 가능한 PSD 파서 `.psb` 도 지원
- [https://github.com/webtoon/psd](https://github.com/webtoon/psd)

### **[elasticsearch-js 8.1.0: Official Elasticsearch Client for Node](https://github.com/elastic/elasticsearch-js)**

- [ES 8.1](https://www.elastic.co/guide/en/elasticsearch/client/javascript-api/8.1/changelog-client.html) 호환

### [fastify-websocket: Basic WebSocket Support for Fastify](https://github.com/fastify/fastify-websocket)

- fastify 에서 만든 fastify 를 위한 웹소켓 지원

# Javascript

### **[React 18 Release Candidate Released](https://reactjs.org/blog/2022/03/08/react-18-upgrade-guide.html)**

- ReactDOM.render ⇒ createRoot 등 렌더링 API 업데이트
- IE 지원 중단

### **[WebGPU — All of the Cores, None of the Canvas](https://surma.dev/things/webgpu/)**

- GPU에 대한 설명과 웹 GPU의 동작 방식, 각종 용어 해설
- 크롬 WebGPU팀이 **`[@webgpu/types](https://www.npmjs.com/package/@webgpu/types)` 를** 유지 관리. API 탐색에 유용

### **[why JS and Swift disagree on when January 1, 1 AD actually was](https://twitter.com/bjhomer/status/1499821210191872000)**

- 그레고리력이 처음 제정되었을 때 춘분점(vernal equinox)을 올바른 위치로 되돌리기 위해 1582년 10월 4일 다음날이 1582년 10월 15일
- swift는 이 부분을 구현하여 1582년 10월15일 전날이 10월 4일 (js는 10월14일)
- JS는 1582년 10월 15일 이전에는 율리우스력을 사용해서 윤년의 계산이 다름

### Release

- **[Partytown 0.5.0](https://github.com/BuilderIO/partytown/releases/tag/v0.5.0)**
- **[AVA 4.1.0](https://github.com/avajs/ava/releases/tag/v4.1.0)**
- **[Rollup.js 2.70.0](https://github.com/rollup/rollup/releases/tag/v2.70.0)**

### [How to Build a File Upload Service with Vanilla JavaScript](https://blog.logrocket.com/how-to-build-file-upload-service-vanilla-javascript/)

- Vanilla JS로 업로드 청크로 분할하여 스트리밍 업로드하기

### [A Complete Guide to TypeScript’s `never` Type](https://www.zhenghao.io/posts/ts-never)

- type is a set of possible values. `never` is an empty set of values.

### **[Tygo: Generate TypeScript Types from Go(lang) Source Code](https://github.com/gzuidhof/tygo)**

- golang 소스 코드를 읽어 ts type을 만들어내는 도구