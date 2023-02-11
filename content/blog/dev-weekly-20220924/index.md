---
title: dev-weekly 2022-09-24
date: "2022-09-24T12:30:00.000Z"
description: "dev-weekly 2022-09-24"
tags: ["javascript", "css", "node"]
---
# CSS

### **[The Power of CSS Blend Modes](https://cloudfour.com/thinks/the-power-of-css-blend-modes)**

- blend 모드를 활용해 이미지 필터 만들기

### **[When is it OK to Disable Text Selection?](https://css-tricks.com/when-is-it-ok-to-disable-text-selection)**

- `user-select: none` 의 적절한 값들과 사용처
- 셀렉션 영역의 비 텍스트를 제거하거나, 우발적 선택 방지, 저작권 컨텐츠 보호 등

### **[Dreamy Blur](https://yuanchuan.dev/dreamy-blur)**

- filter 프로퍼티와 svg필터를 이용한 이미지 필터(레이어를 겹쳐서)
- svg 필터의 각 커맨드는 기본적으로 이전 명령의 출력을 입력으로 사용

### **[Dominant Hand Respecting Design](https://kittygiraudel.com/2022/09/14/dominant-hand-respecting-design)**

- 유저가 주로 사용하는 손을 감지하여 터치 영역을 조정하는 아이디어
- 저자도 좋은 아이디어 일지 확신하지 못함
- [https://clarity.microsoft.com/](https://clarity.microsoft.com/)

# Node

### **[Shell Scripting with Node.js](https://exploringjs.com/nodejs-shell-scripting/)**

- Axel 이 지금까지 작성한 노드 글을 모아 책으로 출간
- [https://exploringjs.com/nodejs-shell-scripting/toc.html](https://exploringjs.com/nodejs-shell-scripting/toc.html)

### **[Real World Node.js Native Binary Compilation with `pkg`](https://www.pulumi.com/blog/nodejs-binaries-with-pkg/)**

- vercel/pkg 를 사용하여 nodejs 네이티브 바이너리 컴파일

### **[Systemd support is now available in WSL](https://devblogs.microsoft.com/commandline/systemd-support-is-now-available-in-wsl/)**

- systemd에 대한 설명 및 어떻게 지원가능한지 설명
- 지원 범위 및 설정방법 (wsl 0.67.6 이상에서 지원, 윈10 wsl2에선 미지원)

### **[DOCX 7.5: Generate Word `.docx` Files from Node or Browser](https://docx.js.org/#/)**

- Node 혹은 브라우저에서 .docx 파일을 생성하는 도구 DOCX 7.5 릴리즈
- https://github.com/dolanmiu/docx/releases/tag/7.5.0

# Javascript

### **[Tesseract.js 3.0: Pure JS OCR for Over 100 Languages](https://tesseract.projectnaptha.com/)**

- OCR 도구 Tesseract.js 3.0 릴리즈 - 러닝 타임 84% 감소, 지원되는 경우 SIMD 사용

### **[A Proposed JS Feature: Extractor Objects](https://github.com/tc39/proposal-extractors)**

- Extractor Object 스테이지1
- [https://tc39.es/process-document/](https://tc39.es/process-document/)

### **[Web based authentication now works for all npm commands](https://github.blog/changelog/2022-09-20-web-based-authentication-now-works-for-all-npm-commands/)**

- CLI 8.19.1 부터 npm login, npm publish 등에 `--auth-type=web` 을 사용하여 웹 기반 인증 가능

### **[Type-Level TypeScript: The Basics](https://type-level-typescript.com/)**

- TS의 기본 컨셉들을 소개하고, Type 문제를 풀어볼 수 있는 REPL제공
- 솔루션도 같이 제공, 문제를 풀면 폭죽 이펙트