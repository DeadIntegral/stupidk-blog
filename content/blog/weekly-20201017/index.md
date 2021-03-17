---
title: javascript weekly 2020-10-17
date: "2020-10-17T09:30:00.000Z"
description: "javascript weekly 2020-10-17"
tags: ["javascript"]
---

# webpack 5 Released
<a href="https://webpack.js.org/blog/2020-10-10-webpack-5-release/" target="_blank">webpack 5 Released</a>
- 웹팩 5 릴리즈
- 캐시(성능)을 크게 개선
- 트리쉐이킹 개선 - 번들 사이즈 감소
- automatic Node polifill 제거
- https://www.taniarascia.com/how-to-use-webpack/

# npm 7.0 Released
<a href="https://github.blog/2020-10-13-presenting-v7-0-0-of-the-npm-cli/" target="_blank">npm 7.0 Released</a>
- 노드15와 같이 퍼블리싱
- workspace : 루트 디렉토리에서 여러 패키지를 관리할 수 있도록 지원
- Automatically installing peer dependencies
- package-lock v2 and support for yarn.lock
- npx, npm, exec 재작성
- npm audit humen-readable

# Babel 7.12.0 Released with TypeScript 4.1 Beta Support and More
<a href="https://babeljs.io/blog/2020/10/15/7.12.0" target="_blank">Babel 7.12.0 Released with TypeScript 4.1 Beta Support and More</a>
- 바벨 7.12.0 릴리즈
- ts4.1의 template literal types, key remapping in mapped types 에 대한 지원,
- ECMA proposal의 class static blocks, imports and exports with string names 구현
- 웹팩 5 지원 - 위 포스트엔 보이지 않는데 소개글엔 존재

<hr>

# Quick bytes

## https://ionicframework.com/blog/announcing-ionic-vue/
- 아이오닉 뷰 출시
- 뷰3로 ios, andriod, pwa 빌드

## https://nodejs.org/en/blog/release/v14.14.0/
- 노드 14.14.0 릴리즈

<hr>

# Don't Copy Paste Into A Shell – Here's Why
<a href="https://briantracy.xyz/writing/copy-paste-shell.html" target="_blank">Don't Copy Paste Into A Shell – Here's Why</a>
- 브라우저 Clipboard API 를 이용하여, 보이는 shell 이 아닌 다른 shell이 복사되도록 하는 코드

<hr>

# Code & Tools

## https://github.com/TimvanScherpenzeel/detect-gpu
- gpu에 따라 다른 렌더링을 위한 라이브러리
- user agent 보다 강력

## https://mtg.github.io/essentia.js/
- js(ts) + cpp(wasm) 을 통한 실시간 및 오프라인, 음악/오디오 분석 및 처리기