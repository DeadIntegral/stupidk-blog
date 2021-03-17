---
title: javascript weekly 2020-05-16
date: "2020-05-16T09:00:00.000Z"
description: "javascript weekly 2020-05-16"
tags: ["javascript"]
---

# Playwright 1.0: Fast and Reliable Cross-Browser Testing
<a href="https://medium.com/@arjunattam/fast-and-reliable-cross-browser-testing-with-playwright-155c0e8a821f" target="_blank">Fast and reliable cross-browser testing with Playwright</a>
- 이전에 MS에서 퍼펫티어 대체하겠다고 내놓은 playwright 소개
- 안정성 향상, 병렬실행, 웹 자동화(PWA 기능 일부 지원)


# Recoil: An Exprimental State Management Library for React 
<a href="https://recoiljs.org/" target="_blank">A state management library for React</a>
- 페북에서 나왔기 때문이 아니라, 최신 React Standard를 따르기 때문에 좋습니다.
- 한글 튜토리얼 https://github.com/alstn2468/Recoil_Tutorial

# Quick bytes
## https://moxon6.github.io/cobol-js-emscripten/
- wasm cobol pong 게임. cobol을 c로 불러와서 emscripten을 통해 wasm으로 컴파일

## https://www.kite.com/blog/product/kite-launches-ai-powered-javascript-completions/
- AI를 통한 JS 자동완성.


# Standard IO: Under the Hood 
<a href="https://keleshev.com/standard-io-under-the-hood" target="_blank">Standard IO: Under the Hood </a>
- console.log를 호출했을 때 실제로 발생하는 일 (v8 기준)


# Now Up to 4GB of Memory in WebAssembly Applications on V8
<a href="https://v8.dev/blog/4gb-wasm-memory" target="_blank">Up to 4GB of memory in WebAssembly</a>
- WASM은 32비트 주소를 사용합니다.
- 첫 번째 이슈는 v8 이 typed array에서 sims를 사용한다는 점입니다.(32비트 signed)
- 두 번째 이슈는 js가 객체 노테이션을 특수하게 처리해야 하는 점입니다.
- emscripten의 메모리 접근 코드는 다음과 같습니다.
```
HEAP32[(ptr + offset) >> 2]
```
- >> 2 부분이 2GB보다 큰 입력이 있을 때 저 부분이 signed 부분을 읽게되고 오버플로가 발생합니다.
- 이 부분을 >>> 로 읽어서 오버플로를 제거


# Code & Tools

## ESLint v7.0.0 Released 
<a href="https://javascriptweekly.com/link/88515/4e4af8cb63" target="_blank">ESLint v7.0.0 released</a>
- node 8 지원 중단
- commonJS 룰 사용안함, bigint 인식, recommend 추가


## Shifty: A Teeny Tiny Tweening Engine 
<a href="https://jeremyckahn.github.io/shifty/doc/" target="_blank">Shifty: A Teeny Tiny Tweening Engine </a>
- Speed: 성능최적화가 잘 되어있고, greensock에 필적하는 애니메이션을 렌더링합니다.
- Flexibility and extensibility: law-level API를 제공하고, 파이프라인으로 연결할 수 있습니다.
- Small footprint: gzipped압축하면 5kb 미만입니다.