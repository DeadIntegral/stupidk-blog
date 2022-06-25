---
title: dev-weekly 2022-01-29
date: "2022-01-29T08:00:00.000Z"
description: "dev-weekly 2022-01-29"
tags: ["javascript", "node", "css", "go"]
---

# CSS

### **[CSS Fingerprint](https://csstracking.dev/)**

- JS와 쿠키에 대한 의존성이 없어서 NoScript, VPN, 브라우저 확장의 추적 방지를 회피
- [https://github.com/OliverBrotchie/CSS-Fingerprint](https://github.com/OliverBrotchie/CSS-Fingerprint)

# Node

### **[Can `process.on('multipleResolves')` Be Deprecated?](https://twitter.com/i/web/status/1486045217635643396)**

- `process.on('multipleResolves')` 의 디프리케이트 전 커뮤니티(트위터)에서 설문조사

### [Announcing TypeScript 4.6 Beta](https://devblogs.microsoft.com/typescript/announcing-typescript-4-6-beta/)

- [TypeScript Trace Analyzer](https://www.npmjs.com/package/@typescript/analyze-trace)
- Breaking Changes
    - Object Rests Drop Unspreadable Members from Generic Objects

# Javascript

### **[On Porting the TypeScript Compiler to Go (vs Rust)](https://kdy1.dev/posts/2022/1/tsc-go)**

- SWC를 만든 사람의 TypeChecker Go 포팅
- [https://news.ycombinator.com/item?id=30074414](https://news.ycombinator.com/item?id=30074414)

### **[Unimported: Find and Fix Dangling Files and Unused Dependencies](https://github.com/smeijer/unimported)**

- 사용하지 않는 파일 검색기

### **IN BRIEF**

- [Deno 2021 진행상황](https://deno.com/blog/deno-in-2021)
- [Angular 2021 진행상황](https://blog.angular.io/angular-2021-recap-and-2022-preview-cb3067f76217)
- **[React Native 0.67](https://reactnative.dev/blog/2022/01/19/version-067)**

### **[React Server Components: A Primer](https://blog.plasmic.app/posts/how-react-server-components-work/)**

- SSR과 차이, 극복하고자 하는 문제, 기본적인 작동방식 등
- 직렬화에 대한 이슈 - react-server-dom-webpack **(**feat.webpack)

### **[What’s New with the DevTools?](https://www.smashingmagazine.com/2022/01/devtools-updates-2022/)**

- 브라우저별 개발자 도구 신기능
    - 크롬 - 레코더
    - 엣지 - DOM 메모리 누수 디버그 도구 Detached Elements
    - 파폭 - 콘솔에서 실행 컨텍스트(iframe) 선택
- 개발자도구 요소 선택기에서도 `pointer-events:none` 는 선택 안되는 이슈 ⇒ `shift` 누르면 선택 가능하게 변경

### **[Animate Anything Along an SVG Path](https://tympanus.net/codrops/2022/01/19/animate-anything-along-an-svg-path/)**

- 경로를 따라 움직이는 애니메이션 만들기

# Go

### **[go-binsize-treemap: Render a Visualization of Go Executable Space Usage](https://github.com/nikolaydubina/go-binsize-treemap)**

- go 바이너리 파일의 구성요소를 SVG 트리맵으로 만들어주는 도구

# ETC

### [JS Framework Performance Table](https://krausest.github.io/js-framework-benchmark/2021/table_chrome_96.0.4664.45.html)

### [Github open issue - commit phishing](https://github.com/torvalds/linux/tree/8bcab0346d4fcf21b97046eb44db8cf37ddd6da0)

- 메일을 변조해서 커밋하는 피싱 - GPG 서명을 통한 대안 존재
- [https://news.ycombinator.com/item?id=24976138](https://news.ycombinator.com/item?id=24976138)