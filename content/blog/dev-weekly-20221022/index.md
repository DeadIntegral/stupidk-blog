---
title: dev-weekly 2022-10-22
date: "2022-10-22T11:00:00.000Z"
description: "dev-weekly 2022-10-22"
tags: ["javascript", "css", "node"]
---
# CSS

### **[CSS-Only Type Grinding: Casting Tokens (sm|md|etc) into Useful Values](https://www.bitovi.com/blog/css-only-type-grinding-casting-tokens-into-useful-values)**

- `@property` 를 이용하여 CSS 만으로 type 삽입

### **[CSS Halftone Patterns](https://css-irl.info/css-halftone-patterns)**

- CSS로 하프톤 패턴 만들기

### **[SVG sprites: old-school, modern, unknown, and forgotten](https://pepelsbey.dev/articles/svg-sprites)**

- SVG 스프라이트하는 다양한 방법 및 이슈들

### **[Learn Accessibility](https://web.dev/learn/accessibility/)**

- web.dev의 접근성 문서

### **[Satori](https://github.com/vercel/satori)**

- vercel에서 만든 HTML,CSS to SVG 도구
- SVG, PNG, PDF export 지원

### **[Vanilla Colorful](https://github.com/web-padawan/vanilla-colorful)**

- 2.7kb의 작은 사용자 지정 색상 선택기
- 리액트, 앵귤러, 뷰, 스벨트, Lit 등 다양한 도구에 삽입하는 예제 제공

# Node

### **[Node.js 19 Released](https://nodejs.org/en/blog/announcements/v19-release-announce/)**

- http(s)/1.1 KeepAlive default true
- stable WebCrypto API
- V8 10.7 지원 (Intl.NumberFormat)

### **[PowerShell, NPM Scripts, and Silently Dropped Arguments](https://www.lloydatkinson.net/posts/2022/powershell-npm-scripts-and-silently-dropped-arguments/)**

- Windows10 파워쉘에서 npm command —인자1 인자2 를 사용하면 인자2가 사라지는 버그

### **[Sending UDP Messages without DNS Lookups](https://hermanradtke.com/sending-udp-messages-in-nodejs-without-dns-lookups/)**

- Nodejs에서 dns.lookup() 없이 UDP 메시지 전송하기
- dns.lookup은 libuv의 스레드 풀에서 실행되는 함수를 동기실 호출하기 때문에 지양

### Release

- [Nx 15.0](https://github.com/nrwl/nx/releases/tag/15.0.0)
- [google translate 2.0](https://github.com/iamtraction/google-translate/releases/tag/v2.0.0)

# Javascript

### **[Metaprogramming with the 2022-03 Decorators API](https://2ality.com/2022/10/javascript-decorators.html)**

- decorator 스테이지3. 바벨은 지원중, TS에서도 곧 지원

### **[why his team is 'breaking up' with CSS-in-JS](https://dev.to/srmagura/why-were-breaking-up-wiht-css-in-js-4g9b)**

- CSS in JS의 장단점 및 작동원리 심층분석

### **[Secure JavaScript URL Validation](https://snyk.io/blog/secure-javascript-url-validation/)**

- 안전한 URL 검사방법
- 실제 취약점 및 해결방법

### **[Why Does `JSON.parse` 'Corrupt' Large Numbers?](https://jsoneditoronline.org/indepth/parse/why-does-json-parse-corrupt-large-numbers/)**

- JSON.parse는 JS를 따라가기 때문에 JS에서 표현하지 못하는 숫자들(큰 정수, 소수 등)은 표현 불가
- JSON Editor online에서는 지원

### **[TypeRunner: A High-Performance TypeScript Compiler](https://github.com/marcj/TypeRunner)**

- 고성능 TS 컴파일러
- 목표, 만드는 목적, 방향성 및 MS와의 방식 차이 등