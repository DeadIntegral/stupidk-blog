---
title: javascript weekly 2020-11-28
date: "2020-11-28T10:00:00.000Z"
description: "javascript weekly 2020-11-28"
tags: ["javascript"]
---

## Flash Animations Live Forever at the Internet Archive
<a href="http://blog.archive.org/2020/11/19/flash-animations-live-forever-at-the-internet-archive/" target="_blank">Flash Animations Live Forever at the Internet Archive</a>
- flash player emulator Ruffle by rust
- 플래시의 간략한 역사와 wasm으로 플래시를 에뮬레이트 해주는 ruffle에 대하여

## TypeScript Performance Tips
<a href="https://github.com/microsoft/TypeScript/wiki/Performance" target="_blank">TypeScript Performance Tips</a>
- TS Performance tip 이라고 하지만, ms서 만든 슈가를 쓰지 않으면 된다는 내용
	- 슈가를 만들어놓고 쓰지 말라해서 비판이 나옴

## TypeScriptToLua: Write Lua with TypeScript
<a href="https://typescripttolua.github.io/" target="_blank">TypeScriptToLua: Write Lua with TypeScript</a>
- TS to Lua
- Redis, Nginx 등에 스크립트를 삽입할 때 사용하기 좋아 보임

<hr>

# Tutorials

## Optimizing Your Pages for the Back/Forward Cache
<a href="https://web.dev/bfcache/" target="_blank">Optimizing Your Pages for the Back/Forward Cache</a>
- Backward Cache 에 대한 브라우저 지원
- 전체 페이지에 대한 스냅샷. 뒤로가기시 새로 요청하지 않음
	- 브라우저가 보류중인 타이머 및 promise를 일시중지 하고 캐시에서 복원될 때 작업처리 재개
- pageshow, pagehide 이벤트로 bfcache에 나오고 들어가는걸 감지 가능
	- unload 이벤트를 사용하지 말 것

## How I Built and Deployed a Fun Serverless Machine Learning App
<a href="https://towardsdatascience.com/building-and-deploying-cartoonify-b4786b382d7e" target="_blank">How I Built and Deployed a Fun Serverless Machine Learning App</a>
- GAN을 사용한 앱 튜토리얼
- GAN + Netlify + Docker + torch

# Code & Tools

## reading-time: Medium-Like Reading Time Estimation
<a href="https://github.com/ngryman/reading-time" target="_blank">reading-time: Medium-Like Reading Time Estimation</a>
- 읽는데 얼마나 걸릴지 측정 해주는 라이브러리
