---
title: javascript weekly 2021-01-16
date: "2021-01-16T08:40:00.000Z"
description: "javascript weekly 2021-01-16"
tags: ["javascript"]
---

## The State of JS 2020 Survey Results
<a href="https://2020.stateofjs.com/ko-KR/" target="_blank">The State of JS 2020 Survey Results</a>
- state of JS 2020 설문조사 결과 - 한글 지원


## Announcing TypeScript 4.2 Beta
<a href="https://devblogs.microsoft.com/typescript/announcing-typescript-4-2-beta/" target="_blank">Announcing TypeScript 4.2 Beta</a>
- typescript 4.2 beta 발표
- rest 문법을 어디서나 사용 가능
	```javascript
	let bar: [boolean, ...string[], boolean];
	```

## Snowpack v3.0: Reimagining Web Development with ESM
<a href="https://www.snowpack.dev/posts/2021-01-13-snowpack-3-0" target="_blank">Snowpack v3.0: Reimagining Web Development with ESM</a>
- 스노우팩 3.0 릴리즈 겸 1.0 릴리즈 1주년
- Streaming Imports
- JS API - SSR helper
- NodeJS Runtime
	- 스벨트팀과의 협업 중 리치 해리스가 서버측 런타임 제작

## Node Package Maintainers, Get Ready For ES Modules
<a href="https://blog.sindresorhus.com/get-ready-for-esm-aa53530b3f77" target="_blank">Node Package Maintainers, Get Ready For ES Modules</a>
- 2021년 4월 노드10 지원 종료. 노드 12부터는 ESM Full support. 마이그레이션 할 적기

<hr>

# Tutorials

## Advanced Promise Patterns: Promise Memoization
<a href="https://www.jonmellman.com/posts/promise-memoization" target="_blank">Advanced Promise Patterns: Promise Memoization</a>
- 요청에 대한 응답을 캐시할 때 요청이 지연될 수 있음
- 응답이 아니라, promise 를 memoization 하기

## How to Implement An Exponential Backoff Retry Strategy
<a href="https://advancedweb.hu/how-to-implement-an-exponential-backoff-retry-strategy-in-javascript/" target="_blank">How to Implement An Exponential Backoff Retry Strategy</a>
- Backoff Retry 전략
	- 동일한 시간으로 리트라이를 계속 하면 서버의 과부하가 심해질 수 있으니 지수를 사용하라는 포스트
- https://github.com/vercel/async-retry 참조하기

## 10 Best Practices to Containerize Node Webapps with Docker
<a href="https://snyk.io/blog/10-best-practices-to-containerize-nodejs-web-applications-with-docker/" target="_blank">10 Best Practices to Containerize Node Webapps with Docker</a>
- 도커 이미지에 프로덕션 종속성만 설치하기
- 프로덕션을 위한 도구 최적화
- 컨테이너를 루트로 실행하지 않기
- 안전한 종료를 위한 이벤트 처리
- 보안 취약성 수정
- 멀티 스테이지 빌드
- ...

## The navigator.clipboard API
<a href="https://davidwalsh.name/navigator-clipboard-api" target="_blank">The navigator.clipboard API</a>
- document.execCommand('copy') 대신 navigator.clipboard 사용하기
- 단, localhost와 https에서만 작동

# Code & Tools

## Merge Chance: Will Your Pull Request Get Merged?
<a href="https://merge-chance.info/" target="_blank">Merge Chance: Will Your Pull Request Get Merged?</a>
- 외부에서 pull request를 날렸을 때 merge되는 비율을 표시해주는 사이트
- 당일 기준 redis 83%, react 44%, vue 23%

## Compiled: Build Time Atomic CSS-in-JS
<a href="https://compiledcssinjs.com/" target="_blank">Compiled: Build Time Atomic CSS-in-JS</a>
- 아틀라시안 랩에서 만든 css in js 도구

## svelte-dnd-action: An Action-Based Drag and Drop Container for Svelte
<a href="https://github.com/isaacHagoel/svelte-dnd-action" target="_blank">svelte-dnd-action: An Action-Based Drag and Drop Container for Svelte</a>
- 스벨트 DnD
- https://svelte.dev/repl/e2ef044af75c4b16b424b8219fb31fd9?version=3.22.2

## vno: A Vue / Deno Love Story?
<a href="https://itnext.io/vno-a-vue-deno-love-story-a9dd4d130ac7" target="_blank">vno: A Vue / Deno Love Story?</a>
- deno 런타임에서 vue 컴파일, 번들링 하는 빌드 도구
