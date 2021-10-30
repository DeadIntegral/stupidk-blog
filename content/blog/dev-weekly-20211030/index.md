---
title: dev-weekly 2021-10-30
date: "2021-10-30T17:00:00.000Z"
description: "dev-weekly 2021-10-30"
tags: ["javascript", "node", "css"]
---

# CSS

### **[Pure CSS Custom Styled Radio Buttons](https://moderncss.dev/pure-css-custom-styled-radio-buttons)**

- css만으로 radio button custom하기 - CSS로 다시 그리기

### **[Photoshop’s Journey to the Web](https://web.dev/ps-on-the-web)**

- Adobe도 웹용 포토샵 제작
- Emscripten을 사용한 WASM

### **[Single Div CSS Hungry Hippo](https://codepen.io/lynnandtonic/pen/NWgQLYP)**

- 하나의 div에 CSS만으로 그린 하마

# Node

### **[Supercharging Node with Rust](https://yieldcode.blog/supercharge-nodejs-with-rust/)**

- 러스트로 작성한 코드를 노드에서 실행가능하도록 만드는 도구 Neon
- 실행할 os와 동일한 환경에서 구축해야 함

### **[How ua-parser-js, an npm Package with 8M+ Weekly Downloads, Was (Briefly) Compromised](https://portswigger.net/daily-swig/popular-npm-package-ua-parser-js-poisoned-with-cryptomining-password-stealing-malware)**

- 주간 다운로드 800만 라이브러리 ua-parser-js가 암호화폐 채굴 및 암호 추출 멀웨어 감염
- 패키지 개발자는 NPM 계정 도용 및 패키지 하이재킹이라고 의심
- 0.7.29, 0.8.0, 1.0.0

### **[Next.js 12 Released](https://nextjs.org/blog/next-12)**

- Rust Compiler - ~3배 빠른 새로고침, ~5배 빠른 빌드
    - SWC 기반 - Babel보다 17배 빠름, Terser보다 7배 빠름
    - 웹팩에 대한 개선 사항 적용
- React 18 지원
- `<Image />` AVIF 지원
- Bot-aware ISR Fallback - SEO 최적화
- Native ES Module 지원

### **[Git Bisect: Travel Through Time and Bugs](https://remimercier.com/how-to-use-git-bisect/)**

- 언제 깨졌는지 알지 못할 때 보다 효율적인 디버깅 방법

# Javascript

### **[What Every JavaScript Developer Should Know About Unicode](https://dmitripavlutin.com/what-every-javascript-developer-should-know-about-unicode/)**

- JS는 UTF-16
- 유니코드의 code unit, surrogate pair, combining marks
- JS의 유니코드 Escape sequences, string comparison, string length, character positioning Regex match