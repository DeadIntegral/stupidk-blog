---
title: dev-weekly 2023-01-28
date: "2023-01-28T12:10:00.000Z"
description: "dev-weekly 2023-01-28"
tags: ["javascript", "node", "css"]
---
# CSS

### **[The Truth About CSS Selector Performance](https://blogs.windows.com/msedgedev/2023/01/17/the-truth-about-css-selector-performance)**

- MS Edge를 이용하여 CSS 셀렉터 사용량 측정하기

### **[Sibling Scopes in CSS, thanks to *:has()*](https://www.bram.us/2023/01/12/sibling-scopes-in-css-thanks-to-has)**

- `.from ~ :has(~ .to)` 를 사용하여 특정 엘리먼트부터 특정 엘리먼트까지의 범위 지정하기(sibling scope)
- only CSS를 통한 캘린더 날짜선택기 예제

# Node

### **[Building Reliable Distributed Systems in Node](https://temporal.io/blog/building-reliable-distributed-systems-in-node)**

- 분산 시스템의 문제를 해결하기 위해 사용하는 durable execution 소개
- [Temporal.io](http://Temporal.io) 를 통해 durable한 서비스 만드는 예제

### **[First Beta of Eleventy v2.0 Released](https://www.11ty.dev/blog/eleventy-v2-beta/)**

- static site generate 도구 Eleventy 2.0 릴리즈
- 의존성 모듈 감소(노드 모듈 용량 1.0.2 버전 대비 77.8% 감소), 향상된 빌드 성능

### **[Packaging *Rust* Apps for the npm Registry](https://blog.orhun.dev/packaging-rust-for-npm/)**

- npm 에 다른 언어 패키지 퍼블리싱하는 과정

### **[s3fs: Drop-In AWS S3 Backed `fs` Replacement](https://github.com/cyclic-software/s3fs)**

- s3에서 nodejs fs 신택스 사용하도록 해주는 도구

### Release

- [node 19.5.0](https://nodejs.org/en/blog/release/v19.5.0/)
- [deno v1.30.0](https://deno.com/blog/v1.30) - built in nodejs 모듈 지원, importMap 지원, api 변경사항 등

# Javascript

### **[Astro 2.0: The Next-Gen 'Islands'-Oriented Web Framework](https://astro.build/blog/astro-2/)**

- 하이브리드 렌더링, 에러 리디자인, 개발서버 최적화(HMR), vite 4.0 적용, open roadmap

### **[Announcing TypeScript 5.0 Beta](https://devblogs.microsoft.com/typescript/announcing-typescript-5-0-beta/)**

- TS 5.0 베타
- 새로운 데코레이터, const Type Parameters, union enum
- `export type *`, jsDoc에서 `@satisfies`, `@overload`  지원
- 4.9 대비해서 용량, 시작 시간, 빌드 타임 등 감소

### **[Getting Started with SvelteKit](https://css-tricks.com/getting-started-with-sveltekit/)**

- 스벨트킷 프로젝트 시작하기

### **[Using .NET Code from JavaScript using WebAssembly](https://www.meziantou.net/using-dotnet-code-from-javascript-using-webassembly.htm)**

- .NET 7부터는 Blazor없이 JS에서 .NET 실행

### Release

- **[React Router 6.8](https://github.com/remix-run/react-router/releases/tag/react-router%406.8.0)** - <Link to=””> 에 absolute url을 넣어도 origin 확인하여 알아서 client side nav로 처리
- **[Cypress 12.4](https://docs.cypress.io/guides/references/changelog#12-4-0) -** 컴포넌트 테스트에서 vite 4.0 지원, 메모리관리 개선옵션, cy.log에서 newline 지원