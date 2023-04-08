---
title: dev-weekly 2022-11-19
date: "2022-11-19T12:00:00.000Z"
description: "dev-weekly 2022-11-19"
tags: ["javascript", "css", "node"]
---

# CSS

### **[The Evolution of Scalable CSS](https://frontendmastery.com/posts/the-evolution-of-scalable-css)**

- CSS의 방법론의 역사

### **[The Math Behind Nesting Rounded Corners](https://cloudfour.com/thinks/the-math-behind-nesting-rounded-corners)**

- 중첩된 border radius를 그릴 때 팁 `outerRadius - gap = innerRadius`

### **[Colorize](https://palette.fm/)**

- 흑백 이미지를 올리면 색칠해주고, 이미지의 스타일을 변경 가능한 온라인 도구

# Node

### **[Deno 1.28 Released (Now with 1.3 Million New Modules..?)](https://deno.com/blog/v1.28)**

- npm 호환성 안정화 - 130만개 이상의 npm 모듈 사용 가능
- 보안 - 의존성이 시스템에 액세스 시도 시 알려주고 제한할 수 있음
- V8 10.9 업그레이드

### **[Node v19.1.0 (Current) Released](https://nodejs.org/en/blog/release/v19.1.0/)**

- `node:test` 모듈은 mocking 동안 top level `mock` 객체 지원
- `fs.watch` 에 재귀 옵션(`recursive: true`) 지원

### **[Announcing TypeScript 4.9](https://devblogs.microsoft.com/typescript/announcing-typescript-4-9/)**

- TS 4.9 릴리즈. 다음 릴리즈는 5.0

### **[Nuxt 3.0: The Vue.js-Based Webapp Framework](https://nuxt.com/v3)**

- vite, vue3, Nitro, TS지원
- 에버그린 브라우저(크롬, FF, 엣지 최근2개 버전, 사파리 최근1년 버전)와 노드 14,16,18,19 지원

# Javascript

### **[What’s So Great About Functional Programming?](https://jrsinclair.com/articles/2022/whats-so-great-about-functional-programming-anyway/)**

- 함수형 프로그래밍의 장점을 물어보면, 대부분 함수형 프로그래밍이 뭔지를 설명해서 어떤 장점이 있는지 작성한 글
- 코드에 대한 확신을 갖는 것(수학적 보증)

### **[Angular v15 Released](https://blog.angular.io/angular-v15-is-now-available-df7be7f2f4c8)**

- 스탠드얼론 API 개발자 프리뷰를 마치고 안정화
- Router, HttpClient 에서 트리쉐이킹이 가능한 스탠드얼론 API
- Chrome DevTools와 협력하여 스택 트레이스 개선
- 머티리얼 디자인 컴포넌트를 기반으로 한 리팩토링 완료

### **[TanStack Router: A Fully Type-Safe Router](https://tanstack.com/router/v1)**

- 빌트 인 캐시, Param API, Parallel Route Loader, Automatic Prefetching, Pending Elements 등 제공
- gzip기준 10kb 번들 (minify 33kb)

### **[OverlayScrollbars 2.0: JS Scrollbar Plugin to Replace Native Scrollbars](https://kingsora.github.io/OverlayScrollbars/)**

- OverlayScrollbar 2.0 릴리즈. TS로 재작성
- 번들 사이즈 54.2kB ⇒ 29.4kB로 감소 (gizp기준으로는 22.9kB ⇒ 13.8kB)

### **Release**

- **[Capacitor 4.5](https://github.com/ionic-team/capacitor/releases/tag/4.5.0)**
- **[React95 4.0](https://github.com/react95-io/React95/releases/tag/v4.0.0)**
- **[Fastify 4.10](https://github.com/fastify/fastify/releases/tag/v4.10.0)**
- **[Playwright 1.28](https://github.com/microsoft/playwright/releases/tag/v1.28.0)**
- **[Cypress 11.1](https://docs.cypress.io/guides/references/changelog#11-1-0)** - next13지원