---
title: javascript weekly 2020-10-03
date: "2020-10-03T09:30:00.000Z"
description: "javascript weekly 2020-10-03"
tags: ["javascript"]
---

# esbuild: A Super Fast JavaScript Bundler and Minifier
<a href="https://github.com/evanw/esbuild" target="_blank">esbuild: A Super Fast JavaScript Bundler and Minifier</a>
- js bundler and minifier
- 다른 번들러들이 너무 느려서 더 빠를 수 있다는 증명을 위해 제작

# Announcing MobX 6
<a href="https://michel.codes/blogs/mobx6" target="_blank">Announcing MobX 6</a>
- 데코레이터 스탠다드에서 제외
- 문서 재작성
- 브라우저 지원 추가(IE)

<hr>

# Quick bytes

## https://blog.npmjs.org/post/630786103662821376/release-v700-rc0 npm7 Release v7.0.0-rc.0

## https://indepth.dev/the-state-of-rxjs-rxjs-7-and-beyond/ rxjs7

## https://svelte.dev/blog/whats-new-in-svelte-october-2020 스벨트 새로운 기능 월간 잡지
<hr>

# Detached Window Memory Leaks
<a href="https://web.dev/detached-window-memory-leaks/" target="_blank">Detached Window Memory Leaks</a>
- iframe과 같이 분리된 창이 있을 때, 이 창을 끄더라도 참조가 남아있어 메모리 누수가 발생
- 다양한 솔루션 제공
	- Unset references - ex) popup = null
	- Monitor and dispose - ex) popup.addEventListener('pagehide', () => { popup = null;
	- Use WeakRef
	- Communicate over postMessage
	- Avoid references using noopener

# A React Cheatsheet for 2020
<a href="https://dev.to/codeartistryio/the-react-cheatsheet-for-2020-real-world-examples-4hgg" target="_blank">A React Cheatsheet for 2020</a>
- 리액트 치트시트 2020버전

<hr>

# Code & Tools

## https://elderguide.com/tech/elderjs/ 
- Elder.js: A Svelte Framework and Static Site Generator

## https://medium.com/airbnb-engineering/introducing-visx-from-airbnb-fd6155ac4658
- visx is a collection of reusable low-level visualization components. 에어비앤비에서 만든 리액트를 위한 컴포넌트 모음

## https://github.com/elsaland/elsa
- Go로 만든 JS, TS 런타임
- V8 대신 QuickJS를 사용

## https://projects.verou.me/parsel/
- css selector parser
- ::before 와 같은 가상선택자도 선택 가능
- css level4도 사용 가능