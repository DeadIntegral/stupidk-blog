---
title: dev-weekly 2021-12-04
date: "2021-12-04T10:00:00.000Z"
description: "dev-weekly 2021-12-04"
tags: ["node", "javascript"]
---


# Node

### **[Strapi v4: An Open Source Node.js Headless CMS](https://strapi.io/blog/announcing-strapi-v4)**

- 새로운 UI, 플러그인 API, 쿼리 엔진 등이 포함된 v4 릴리즈

### In brief

Github Action이 Node 16 지원

- [https://github.com/actions/runner/releases/tag/v2.285.0](https://github.com/actions/runner/releases/tag/v2.285.0)

# Javascript

### **[asciinema-player, Now 4x Smaller and 50x Faster with JS *and* Rust](https://blog.asciinema.org/post/smaller-faster/)**

- JS + Rust로 다시 구현해서 터미널 인터프리터는 50배 성능 향상, 번들 크기 4분의1로 감소
- 클로저 스크립트에서 발생한 이슈와 마이그레이션한 이유

### **[Mitosis: Write Components Once, Run Everywhere](https://github.com/BuilderIO/mitosis#readme)**

- 리액트, 앵귤러, 뷰, 스벨트, 솔리드 호환되는 컴포넌트 제작 도구
- 리액트와 같은 모습에 훅스와 유사한 신택스를 사용하지만 뷰처럼 뮤터블하고, 솔리드와 같은 스태틱한 JSON 형태로 포맷 후 스벨트처럼 컴파일하고 앵귤러와 유사한 구조를 가짐

### **['Thank You, Angular' (and Thank You, Igor!)](https://blog.angular.io/thank-you-angular-d90d70f2e9d8)**

- 앵귤러 팀 리더 Igor(구글에서 11.5년, 앵귤러에서 12.5년 근무)의 구글퇴사

### **[JSON Modules in JavaScript](https://dmitripavlutin.com/javascript-json-modules/)**

- `import json from "./file.json" asset { type: json };` json module 이제 stage3

### **[Ladda: Buttons with Built-In Loading Indicators](https://lab.hakim.se/ladda/)**

- 로딩바가 포함된 버튼 라이브러리

### **[noUiSlider: Lightweight Range Slider with Full Touch Support](https://refreshless.com/nouislider/)**

- 접근성 챙긴(ARIA + Keyboard) UI슬라이더
- IOS, AOS, Window에서 멀티 터치, 반응형지원, 제로 디펜던시
- GPU animation, no reflow

### **[jsvu: JavaScript (Engine) Version Updater](https://github.com/GoogleChromeLabs/jsvu)**

- JS의 각 엔진들의 다양한 버전을 소스를 받아서 컴파일 하는 대신, 설치해주는 도구