---
title: javascript weekly 2020-10-24
date: "2020-10-24T10:00:00.000Z"
description: "javascript weekly 2020-10-24"
tags: ["javascript"]
---

# React 17.0 Released
<a href="https://reactjs.org/blog/2020/10/20/react-v17.html" target="_blank">React 17.0 Released</a>
- 리액트 17 릴리즈, 문서는 변경 없음

# Node 15 Released
<a href="https://nodejs.medium.com/node-js-v15-0-0-is-here-deb00750f278" target="_blank">Node 15 Released</a>
- 노드15 릴리즈
- AbortController
- N-API Version 7 (주로 네이티브 에드온을 구현하는 사람들이 사용합니다.)
- NPM 7
- Throw on unhandled rejections : 이제 해당 error를 Warn으로 변경할 수 있습니다.
- QUIC(HTTP3 실험적 지원)
- V8 8.6 : Promise.any(), String.prototype.replaceAll()

# Skypack Discover: A Way to Discover and Test Recommended JS Packages
<a href="https://www.skypack.dev/blog/2020/10/introducing-skypack-discover/" target="_blank">Skypack Discover: A Way to Discover and Test Recommended JS Packages</a>
- Skypack v2검색 엔진 출시 (1은 Pika cdn)
- 프로젝트에 적합한 검색을 위해 context를 가져옴 (npm에는 그런게 없어서 디프리케이트된 것을 설치 후 경고나 에러를 받을 수 있음)
- http2,3 지원 및 캐싱, 엣지 캐싱, automatic js polyfill 등 다양한 기능지원
- https://www.skypack.dev/

<hr>

# Quick bytes

## http://www.p01.org/MONOSPACE/
- 어셈블리 2020 우승작. 1021바이트
- http://www.p01.org/MONOSPACE/monospace-compatible.htm

## https://www.youtube.com/watch?v=qSfdtmcZ4d0
- 리치 해리스의 웹 개발의 미래와 Sapper svelte에 대한 토크

## https://github.com/webpack/webpack/releases/tag/v5.2.0
- 웹팩 5.2.0 릴리즈
- 2주만에 5.0.0 에서 5.2.0 까지

<hr>

# Don't Copy Paste Into A Shell – Here's Why
<a href="https://briantracy.xyz/writing/copy-paste-shell.html" target="_blank">Don't Copy Paste Into A Shell – Here's Why</a>
- 브라우저 Clipboard API 를 이용하여, 보이는 shell 이 아닌 다른 shell이 복사되도록 하는 코드

<hr>

# Tutorials
## https://frankforce.com/dissecting-a-dweet-9-city-sunset/
- 140자로 만든 도시 일몰

## Don't Copy Paste Into A Shell – Here's Why
<a href="https://medium.com/nmc-techblog/introducing-the-async-cookie-store-api-89cbecf401f" target="_blank">Don't Copy Paste Into A Shell – Here's Why</a>
- Introducing the Async Cookie Store API (in Chrome 87)
- 새로운 쿠키 API. 기존의 document.cookie 다루는것은 너무 구식.
- https://wicg.github.io/cookie-store

# Code & Tools

## https://github.com/infinitered/nsfwjs
- 텐서플로를 통해 클라이언트 사이드에서 NSFW감지하는 라이브러리

## https://github.com/fingerprintjs/fingerprintjs
- 핑거프린트js v3 출시.
- 완전히 모듈화 하고, TS로 다시 작성.
- please use this for good, not evil 프로젝트

## https://css-tricks.com/working-with-javascript-media-queries/
- js에서 미디어쿼리 사용하기
- resize대비해서 압도적인 성능
- IE10+ 모던 브라우저 전부 지원