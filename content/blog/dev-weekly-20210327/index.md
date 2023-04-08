---
title: dev-weekly 2021-03-27
date: "2021-03-27T10:00:00.000Z"
description: "dev-weekly 2021-03-27"
tags: ["javascript", "css", "go", "node"]
---

# CSS, Node, Go, Etc

## CSS

[Taming Blend Modes: difference and exclusion](https://css-tricks.com/taming-blend-modes-difference-and-exclusion)

- blend가 작동하는 방식을 설명
- 블렌드가 계산되는 수식을 설명
- blend로 표현 가능한 다양한 예제 포함

---

## Node

### **[Piscina: A Fast Worker Thread Pool Implementation](https://github.com/piscinajs/piscina)**

- 노드 워커 쓰레드 풀 구현
- abort controller 를 통한 태스크 캔슬 가능

### **[A Look at Nine JavaScript and TypeScript ORMs](https://www.sitepoint.com/javascript-typescript-orms/)**

- orm에 대한 설명과, 다양한 JS,TS ORM 도구들 예제
- knex, 몽구스, 타입orm, 시퀄라이즈, 프리즈마 등등

### **[Node v15.12.0 (Current) Released](https://nodejs.org/en/blog/release/v15.12.0/)**

- 노드 15.12 릴리즈
- promise 기반의 writeFile, readFile, NAPI v8 안정화
- openssl to quictls/openssl

---

## Go

### **[The Darker Corners of Go](https://rytisbiel.com/2021/03/06/darker-corners-of-go/)**

- go에 대해 더 깊은 이해를 할 수 있는 긴 레슨

---

# Javascript

### **[SvelteKit Now In Public Beta](https://svelte.dev/blog/sveltekit-beta)**

- 리치 해리스의 스벨트킷 글

### **[Billboard.js 3.0: The D3.js-Powered Chart Library](https://netil.medium.com/billboard-js-3-0-release-d3-js-v6-support-new-candlestick-type-9bd74af6a753)**

- 빌보드js 3.0 릴리즈
- D3 v6 지원
- OHLC candle chart 지원
- export() API 향상, 새로운 subchart API

### **Quick Bits**

[https://txtfiddle.com/](https://txtfiddle.com/)

- txtfiddle이라는 새로운 온라인 자바스크립트 샌드박스 에디터
- 여러 코드 예제가 기입된 '템플릿' 이라는 기능
- 실행중인 코드 abort 가능

[https://www.pcjs.org/software/pcx86/sys/windows/3.10/](https://www.pcjs.org/software/pcx86/sys/windows/3.10/)

- 웹에서 돌아가는 윈도 3.1
- 브라우저용 IBM PC 에뮬레이터

---

## Code & Tools

### **[eslint-plugin-clean-regex: ESLint Plugin for Better Regular Expressions](https://github.com/RunDevelopment/eslint-plugin-clean-regex)**

- 정규식 옵티마이즈 해주는 eslint plugin

### **[goober](https://github.com/cristianbote/goober)**

- 1kb 도 안되는 css in js
- devDependency 에 스타일드 컴포넌트 들어가있음