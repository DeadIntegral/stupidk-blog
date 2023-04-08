---
title: dev-weekly 2021-07-10
date: "2021-07-10T14:00:00.000Z"
description: "dev-weekly 2021-07-10"
tags: ["javascript", "node", "deno", "go"]
---

# Node, Deno

## Node

### **[npm audit: Broken by Design](https://overreacted.io/npm-audit-broken-by-design/)**

- 리덕스 제작자 dan이 npm audit 이 프론트 프로젝트에서 잘못 동작하고 있는 예시들을 보여주며 비판하는 글

### **[Node v16.4.2, v14.17.3, and v12.22.3 Released, But You Probably Don't Need Them](https://nodejs.org/en/blog/release/v16.4.2/)**

- windows를 사용하는 비 영어권 이용자들에게 영향을 주는 버그 픽스

### **[Nest 8.0: A Mature Framework for Building Scalable Server-Side Apps](https://github.com/nestjs/nest/releases/tag/v8.0.0)**

- nestjs 8.0 릴리즈

## Deno

### **[Deno Deploy Beta 1](https://deno.com/blog/deploy-beta1)**

- 전 세계 25개 데이터센터에서 멀티 테넌트 v8 엔진으로 deno 배포
- 코드 푸시하는 순간 프로비저닝된 서브도메인에 배포

## Go

### **[Russ Cox on Hardware Memory Models](https://research.swtch.com/hwmm)**

- 하드웨어 메모리 모델

### **[Benchmarks in Go Can Be 'Surprising'](https://leveluppp.ghost.io/benchmarks-in-go-can-be-surprising/)**

- 정확히 동일한 코드가 동일한 시스템의 동일한 코드베이스에서 매우 다른 벤치마크가 나타나는 현상

# Javascript

### **[The State of Web Workers in 2021](https://www.smashingmagazine.com/2021/06/web-workers-2021/)**

- wokers를 수용하기 위한 아키텍처
    - concurrency model - actor
    - concurrency model - shared memory

### **[How export default thing is Different to export { thing as default }](https://jakearchibald.com/2021/export-default-thing-vs-thing-as-default/)**

- 현재 값과 참조 차이

```jsx
// These give you a live reference to the exported thing(s):
import { thing } from './module.js';
import { thing as otherName } from './module.js';
import * as module from './module.js';
const module = await import('./module.js');
// This assigns the current value of the export to a new identifier:
let { thing } = await import('./module.js');

// These export a live reference:
export { thing };
export { thing as otherName };
export { thing as default };
// These export the current value:
export default thing;
export default 'hello!';
```

### **[https://twitter.com/jsjoeio/status/1411369162971045895](https://twitter.com/jsjoeio/status/1411369162971045895)**

- 일정에 따라 스프레드 시트에 삽입한 js 실행하기 (like cron)

## Code & Tools

### **[html2canvas 1.0: A JavaScript HTML Renderer](https://html2canvas.hertzen.com/)**

- 페이지 또는 특정 엘리먼트를 스크린샷 찍어서 캔버스에 렌더링 해주는 도구. 1.0 릴리즈

### **[imask.js: A Vanilla JavaScript Input Mask](https://imask.js.org/)**

- 사용자가 입력한 값들을 밸리데이트 하는 대신에,
잘못된 값 입력 못하게 인풋을 강제하는 도구