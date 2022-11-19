---
title: dev-weekly 2022-10-01
date: "2022-10-01T17:00:00.000Z"
description: "dev-weekly 2022-10-01"
tags: ["javascript", "css", "node"]
---

# CSS

### **[Web Almanac 2022](https://almanac.httparchive.org/en/2022/css)**

- 2022년 웹에서 CSS 사용에 대한 통계들
- 셀렉터, 값과 유닛, 프로퍼티, 색상 이미지, 레이아웃 등 다양한 영역에서의 지표

### **[Use Cases for CSS Comparison Functions](https://ishadeed.com/article/use-cases-css-comparison-functions)**

- Clamp() 에 대한 설명 및 언제 적용해야 할지에 대한 가이드

### **[CSS Rules vs. CSS Rulesets](https://www.impressivewebs.com/css-rules-vs-css-rulesets)**

- CSS 를 작성할 때는 괜찮지만 글을 쓸 때는 바른 용어를 쓰자
    
    ```css
    /* 아래 전체를 rule 혹은 ruleset(rule set) 이라고 함 */
    section { /* 괄호 사이를 데클레이션 블록 */
      margin: 0 20px; /* 이 라인은 개별 데클레이션 */
      color: #888; /* 또다른 데클레이션 */
    }
    ```
    

### **[Why Custom Properties Don’t Work With the url() CSS Function](https://www.stefanjudis.com/today-i-learned/custom-properties-dont-work-with-the-url-css-function)**

- 사용자 정의 변수가 url() 에서 작동하지 않는 이유
- url()과 url(’’)은 다른 구문이고, url()은 함수가 아니라 url(text) 까지가 하나의 토큰
- 이를 위한 솔루션 제안 `-image: url(https://url); background: var(--image);`

### **[Testing Web Design Color Contrast](https://web.dev/testing-web-design-color-contrast)**

- 웹 접근성 만족을 위한 색상 대비 감지 도구들
- 크롬 개발자도구에서 contrast ratio 보는법 및 보정 방법

### **[Markwhen](https://markwhen.com/)**

- mermiad처럼 markdown과 유사한 텍스트를 작성하면 계단식 타임라인으로 만들어주는 도구

### **[Portal (CSS)](https://codepen.io/amit_sheen/pen/mdLOKom)**

- css only로 만들어낸 포탈 애니메이션

# Node

### **[Don’t Worry, Nobody is Replacing Node.js](https://blog.bitsrc.io/dont-worry-nobody-is-replacing-node-js-not-even-bun-and-even-less-deno-4e7148cff78)**

- deno, bun 등 다른 런타임들이 nodejs를 대체하진 않을거라고 주장하는 글

### **[September 23rd 2022 Security Releases](https://nodejs.org/en/blog/vulnerability/september-2022-security-releases/)**

- macOS의 DNS rebinding 보호 이슈
- 멀티 라인 Transfer-Encoding 헤더를 통한 HTTP Request Smuggling

### **[Minimize Heap Allocations in Node.js](https://blog.appsignal.com/2022/09/28/minimize-heap-allocations-in-nodejs.html)**

- 잘못된 부분을 개선하는 v8 엔지니어의 답글 [https://news.ycombinator.com/item?id=33007398](https://news.ycombinator.com/item?id=33007398)
    - JS primitive도 참조로 전달되지만, 이 참조는 값으로 전달되기 때문에 할당해도
    - small integer(Sims)를 제외한 모든 primitive는 힙에 저장

### **[Online Tool to Translate i18next JSON Files](https://translate.i18next.com/)**

- i18next 포맷을 구글 번역으로 value만 번역해주는 도구

### **[textlint: A Pluggable Linting Tool for Text and Markdown](https://textlint.github.io/)**

- 자연어에 대한 lint (영어만 지원)

# Javascript

### **[The Web Almanac 2022's Take on the State of JavaScript in the Real World](https://almanac.httparchive.org/en/2022/javascript)**

- 800만개의 사이트 분석 결과 - JS 사용 현황
    - dynamic import, web worker, worklet
    - compression, minify, 블로킹 타임 등
    - 라이브러리, 취약점 있는 버전 사용중인 도구 등

### **[Announcing TypeScript 4.9 Beta](https://devblogs.microsoft.com/typescript/announcing-typescript-4-9-beta/)**

- `satisfies` 오퍼레이터 추가
- in 오퍼레이터를 통한 프로퍼티 축소

### **[VS Code Timeline Restores Lost Work That Git Can’t](https://austingil.com/vs-code-timeline-restores-work-git-cant/)**

- VSCode에는 타임라인 이라는 기능이 있어, 깃 커밋 없이 저장 시점마다 스냅샷을 저장해줌

### ****[Announcing Turnstile, a user-friendly, privacy-preserving alternative to CAPTCHA](https://blog.cloudflare.com/turnstile-private-captcha-alternative/)****

- UX를 해치지 않는 캡차의 대체 도구 Turnstile 베타
- 더 나은 인터넷을 만드는게 사명이기 때문에 무료로 공개

### ****[Introducing workerd: the Open Source Workers runtime](https://blog.cloudflare.com/workerd-open-source-workers-runtime/)****

- JS/WASM 런타임 워커디(workerd) 공개
- HTTP 서버에 중점을 둔 런타임
- workerd는 나노 서비스 - 라이브러리 호출에 가까운 오버헤드로 독립 배포의 이점

### **[Preview.js: Fast Component Previews in Your IDE](https://previewjs.com/)**

- VSC, IntelliJ(및 웹스톰) 확장. 컴포넌트 단위로 미리보기가 가능
- 타이핑 시점마다 Vite(esbuild)를 통해 빠르게 화면 반영

# Etc

### **[MFA Fatigue(피로) 공격](https://www.ciokorea.com/news/256786)**

- MFA 피로 공격 - 사람에게 지속적으로 MFA 인증을 보내서 피로하게 만들고 내가 원하는 버튼을 클릭하라고 하면 클릭해버리는걸 유도하는 공격

### **[Programmer Competency Matrix](https://sijinjoseph.com/programmer-competency-matrix/)**

- 프로그래머 능력 매트릭스

### **[https://github.com/lennysec/awesome-tls-hacks](https://github.com/lennysec/awesome-tls-hacks)**

- SSL/TLS 보안 관련 리소스 모음