---
title: dev-weekly 2022-03-05
date: "2022-03-05T17:00:00.000Z"
description: "dev-weekly 2022-03-05"
tags: ["javascript", "css", "node"]
---

# CSS

### **[When to Avoid the text-decoration Shorthand Property](https://css-tricks.com/when-to-avoid-css-text-decoration-shorthand)**

- text-decoration은 축약형이고, 이를 설정하면 관련 값들이 초기화되는 이슈 존재
- ex)
    
    ```css
    text-decoration-thickness: 0.08em;
    text-decoration: underline; // text-decoration-thickness가 초기화
    ```
    
- `text-decoration-line: underline;` 를 사용하는 방법

### **[Inspecting Web Views in macOS](https://blog.jim-nielsen.com/2022/inspecting-web-views-in-macos)**

- macOS 앱을 safari web inspector를 트리거해서 개발자도구 사용하기
- 터미널에 write 명령을 입력하여 트리거
    
    ```bash
    defaults write NSGlobalDomain WebKitDeveloperExtras -bool true
    defaults write -g WebKitDeveloperExtras -bool YES
    ```
    

# Node

### **[Running Commands with `execa` in Node](https://blog.logrocket.com/running-commands-with-execa-in-node-js/)**

- Sindre Sorhus의 라이브러리 execa에 대한 소개, `child_process` 대비 장점
- 간단한 사용법

### **[Red Hat and IBM's Node.js 'Reference Architecture'](https://github.com/nodeshift/nodejs-reference-architecture)**

- 고객 및 내부 팀이 Nodejs app 구축에 대한 의견 및 지침 제공
- [https://nodeshift.dev/nodejs-reference-architecture/](https://nodeshift.dev/nodejs-reference-architecture/)

# Javascript

### **[TypeScript 4.6 Released (And It Even Benefits Non-TS Users!)](https://devblogs.microsoft.com/typescript/announcing-typescript-4-6/)**

- 4.6 Release. 4.6RC 와의 차이

### **[VS Code release](https://code.visualstudio.com/updates/v1_65)**

- 디버깅 - Lazy variables
- TS 4.6

### **[How Do Primitive Values Get Their Properties?](https://2ality.com/2022/03/properties-of-primitives.html)**

- primitive value를 객체처럼 사용하는 방법과 프로퍼티가 어디서 오는지

### **[Redux Toolkit 1.8.0 Released](https://github.com/reduxjs/redux-toolkit/releases/tag/v1.8.0)**

- `listenerMiddleware` 추가

### **[dnt: Deno-to-Node Package Transformation Tool](https://github.com/denoland/dnt)**

- Deno 도구를 Node 패키지로 빌드하는 도구