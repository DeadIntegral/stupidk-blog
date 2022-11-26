---
title: dev-weekly 2022-11-26
date: "2022-11-26T11:50:00.000Z"
description: "dev-weekly 2022-11-26"
tags: ["javascript", "css", "node"]
---

# CSS

### **[An Interactive Guide to Flexbox](https://www.joshwcomeau.com/css/interactive-guide-to-flexbox)**

- flexbox layout mode에 대한 joshw의 멘탈 모델 설명
- flex에서의 width는 *hypothetical size*

### **[CSS :where() To Replace Complex Multi-Selectors](https://helloanselm.com/writings/css-where-to-replace-complex-multi-selectors)**

- 복잡한 셀렉터를 `:where()` 로 리팩토링하기
- where와 is는 작동은 같지만, is는 specificity를 증가시킴

### **[The Anatomy of visually-hidden](https://www.tpgi.com/the-anatomy-of-visually-hidden)**

- 접근성을 위해 숨겨진 널리 사용되는 CSS property들에 대한 설명
- width, height를 1px보다 작게하면 접근성 트리에서 사라짐.
- `clip: rect(0 0 0 0);` 을 통해 시각적으로 숨기기

### **[Regex-Vis](https://regex-vis.com/)**

- 정규식을 시각적으로 표현해주는 온라인 도구

### **[City Life - Day & Night - Pure CSS](https://codepen.io/josetxu/pen/poKbEjG)**

- HTML, CSS만으로 표현한 빌딩의 밤낮

# Node

### **[Node.js 18.x Runtime Now Available on AWS Lambda](https://aws.amazon.com/ko/blogs/compute/node-js-18-x-runtime-now-available-in-aws-lambda/)**

- AWS 람다에서 Nodejs18 사용가능
- 람다의 Nodejs 런타임에 AWS SDK v2가 들어가있었으나 v3으로 업그레이드

### **[Producing Native ES Modules on Node.js with TypeScript](https://2ality.com/2021/06/typescript-esm-nodejs.html)**

- TS에서 네이티브 ESM 작동방식 및 설정
- [Cheat sheet module](https://exploringjs.com/impatient-js/ch_modules.html)

### **[Writing and Organizing Node API Tests The Right Way](https://larswaechter.dev/blog/nodejs-api-testing/)**

- 노드에서 API 서버를 테스팅하기

### **[aoi.js 6.0: String-Based Package to Create Discord Bots](https://aoi.js.org/)**

- 디스코드 봇 동작을 특수 형식 문자열로 정의가능한 비개발자가 보다 쉽게 봇을 만드는데 포커싱한 도구

# Javascript

### **[The State of JavaScript 2022 Survey is Open](https://survey.devographics.com/survey/state-of-js/2022)**

- State of JS 2022 설문시작. 이번엔 게스트 참가 가능

### **[Complete rewrite of ESLint Discussion](https://github.com/eslint/eslint/discussions/16557)**

- eslint 제작자의 다시 만들자는 논의
- 런타임 불가지론, 언어 불가지론, 러스트 기반 WASM 등

### **[React Native in 2022 and Beyond](https://semaphoreci.com/blog/react-native)**

- bridge의 일부를 대신할 수 있는 Turbo Modules
- 새로운 렌더러 Fabric, JS Engine 헤르메스
- 플랫폼추가 (데스크탑앱, 웹 등) - [https://microsoft.github.io/react-native-windows/resources-showcase](https://microsoft.github.io/react-native-windows/resources-showcase)
- 커뮤니티 기여 - 각 회사들의 지원

### **[Eruda 2.6: A Console for Mobile Browsers](https://github.com/liriliri/eruda/releases/tag/v2.6.0)**

- 모바일 브라우저 콘솔 도구 Eruda 2.6 릴리즈