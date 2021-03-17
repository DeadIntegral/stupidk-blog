---
title: javascript weekly 2020-11-07
date: "2020-11-07T09:00:00.000Z"
description: "javascript weekly 2020-11-07"
tags: ["javascript"]
---

# What's the Deal with Svelte and SvelteKit?
<a href="https://svelte.dev/blog/whats-the-deal-with-sveltekit" target="_blank">What's the Deal with Svelte and SvelteKit?</a>
- 스벨트는 어떻게 발전하고 있는가?
- sapper 마이그레이션
- 스노우팩을 활용한 DX + 롤업 번들을 통한 앱 최적화

# New, Core 'Redux Fundamentals' Tutorial
<a href="https://redux.js.org/tutorials/fundamentals/part-1-overview" target="_blank">New, Core 'Redux Fundamentals' Tutorial</a>
- redux fundamental 재작성

<hr>

# Quick bytes

## https://hackaday.com/2020/11/02/ttl-simulator-in-javascript/
- JS 회로 시뮬레이터

## https://www.spiderbasic.com/
- Basic to Web(JS) 컴파일러

<hr>

# Tutorials

# Clickjacking Attacks and How to Prevent Them
<a href="https://auth0.com/blog/preventing-clickjacking-attacks/" target="_blank">Clickjacking Attacks and How to Prevent Them</a>
- 클릭재킹 공격은 무엇이고, 어떻게 재현 하는지(깃헙 레포 포함)
- CSRF랑 어떻게 다른가? 방어는 어떻게 하는가
	- X-Frame-Options
	- CSP
	- cookie sameSite origin

# An Introduction to FFmpeg.wasm, a WebAssembly / JS Port of FFmpeg
<a href="https://jeromewu.github.io/ffmpeg-wasm-a-pure-webassembly-javascript-port-of-ffmpeg/" target="_blank">An Introduction to FFmpeg.wasm, a WebAssembly / JS Port of FFmpeg</a>
- ffmpeg wasm버전
- 멀티스레딩을 위한 SharedArrayBuffer 사용
- 스레드 시뮬레이션 때문에 다수의 웹워커가 존재할 수 있음
- 현재는 x86 assem to SIMD assem 이식에 비용 발생

<hr>

# Code & Tools

## Socket.io 3.0 Released: A Realtime Framework for Node and Browser
<a href="https://github.com/socketio/socket.io/releases/tag/3.0.0" target="_blank">Socket.io 3.0 Released: A Realtime Framework for Node and Browser</a>
- Socket.io 3.0 릴리즈

## gron: Make JSON Greppable
<a href="https://github.com/tomnomnom/gron" target="_blank">gron: Make JSON Greppable</a>
- JSON into "grep"pable assignment
- 문서가 안좋은 api도 직접 데이터를 가져오고 파싱하여 이쁘게 변형

## Graphery SVG: A Library for SVG Creation and Management
<a href="https://www.graphery.org/svg/" target="_blank">Graphery SVG: A Library for SVG Creation and Management</a>
- SVG를 간단히 사용할 수 있도록 래핑한 라이브러리
- IE지원안함, 엣지12+

## SpanTree: Adds Tree-Based File Navigation to GitLab
<a href="https://github.com/tavyandy97/span-tree" target="_blank">SpanTree: Adds Tree-Based File Navigation to GitLab</a>
- 깃헙에 옥토트리가 있듯이, 깃랩용 트리 익스텐션

## Marked: A Fast Markdown Parser and Compiler
<a href="https://github.com/markedjs/marked" target="_blank">Marked: A Fast Markdown Parser and Compiler</a>
- 성능을 위한 마크다운 파서 겸 컴파일러
