---
title: dev-weekly 2023-06-02
date: "2023-06-02T23:50:00.000Z"
description: "dev-weekly 2023-06-02"
tags: ["javascript", "css", "node", "etc"]
---
# CSS

### **[Register custom properties in CSS, get and update them with JavaScript](https://fullystacked.net/posts/custom-properties)**

- JS에서 CSS 선언 수정하는 방법들.
- `getComputedStyle(document.documentElement).getPropertyValue('--size');` , `document.documentElement.style.setProperty('--accent-color', 'rgb(100,110,10)');`

# Node

### **[cli utility for querying the node_modules directory](https://github.com/ranyitz/qnm)**

- node_modules 디렉토리에 설치된 모듈의 버전을 빠르게 확인하기 위한 cli 도구

### **[Hands on with the Node.js test runner](https://www.sonarsource.com/blog/node-js-test-runner/)**

- node 20에서 안정된 빌트인 테스트 러너 실습
- 테스트 스킵, 서브테스트, 훅, it/describe 신택스, 리포터 등에 대한 간략한 설명

### **[New reference pages on MDN for JavaScript regular expressions](https://developer.mozilla.org/en-US/blog/regular-expressions-reference-updates/)**

- MDN 정규표현식 페이지 개편

# Javascript

### **[iOS 17 automatically removes tracking parameters from links you click on](https://9to5mac.com/2023/06/08/ios-17-link-tracking-protection/)**

- iOS 17은 링크에서 추적 코드를 자동으로 제거.

### **[News from WWDC23:WebKit Features in Safari 17 beta](https://webkit.org/blog/14205/news-from-wwdc23-webkit-features-in-safari-17-beta/)**

- webApp, model element, webXR, JPEG XL, popover attribute 등 지원
- 오프스크린캔버스 3D, 스토리지 할당량 정책 변경

### **[Polywasm: A Polyfill to Run WASM in JS Environments](https://github.com/evanw/polywasm)**

- WASM 폴리필. 당연히 wasm보다 느리지만 실행 안되는 것 보다 낫기 때문에.

### **[RSC From Scratch. Part 1: Server Components](https://github.com/reactwg/server-components/discussions/5)**

- 댄 아브라모브가 리액트 서버 컴포넌트를 처음부터 다시 만들어가며 그 과정을 설명하는 심층 분석.

### **[eslint-plugin-perfectionist](https://github.com/azat-io/eslint-plugin-perfectionist)**

- 객체, imports, 타입, enum, JSX prop까지 정렬해주는 eslint 플러그인

### **Release**

- **[Tesseract.js 4.1](https://github.com/naptha/tesseract.js/releases/tag/v4.1.0)**
- **[TensorFlow.js 4.7](https://github.com/tensorflow/tfjs/releases/tag/tfjs-v4.7.0)**
- **[Madge 6.1](https://github.com/pahen/madge/releases/tag/v6.1.0)**

# ETC

### **[shapecatcher: Unicode Character Recognition](https://shapecatcher.com/)**

- 캔버스에 무언가를 그리고 검색하면 가장 가까운 유니코드 문자들을 보여주는 서비스

### **[How Chrome achieved high scores on three browser benchmarks](https://blog.chromium.org/2023/06/how-chrome-achieved-high-scores-on.html)**

- 새로운 미드 티어 컴파일러 발표: Maglev (같은 이름의 여러 도구가 이미 존재. 로드밸런서 등)
- speedmeter, motionmark, jetstream의 세 가지 항목에서 크롬이 높은 점수 획득