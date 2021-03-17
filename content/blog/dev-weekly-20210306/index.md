---
title: dev-weekly 2021-03-06
date: "2021-03-06T08:40:00.000Z"
description: "dev-weekly 2021-03-06"
tags: ["javascript", "css", "node", "deno", "go"]
---

# CSS, Node, Deno, GO, DB, ETC

## CSS

### [Pattern Generator](https://doodad.dev/pattern-generator/)

- GUI로 패턴을 생성하고, 이미지나 css background(svg)로 추출하는 서비스

### [Table TenniCSS](https://codepen.io/amit_sheen/pen/PobQjMX)

- HTML, CSS 만든 탁구 애니메이션

## Node

### [array-union 3.0: Create An Array of Unique Values, In Order, From Input Arrays](https://github.com/sindresorhus/array-union)

- 배열을 입력 순서대로 유니크하게 만드는 라이브러리
- 주당 npm 다운로드 2200만(3월 5일 기준)회에 달하고, 이제 pure ESM package에 들어가는 한줄짜리 라이브러리

    ```jsx
    const arrayUnion = (...arguments_) => [...new Set(arguments_.flat())];
    ```

### [Chevrotain 8.0: A Parser Building Toolkit](https://chevrotain.io/docs/)

- SQL-esque 언어에 대한 파서를 빌드하는 과정 안내

### [Node v15.11.0 (Current) Released](https://nodejs.org/en/blog/release/v15.11.0/)

- 노드 15.11.0 릴리즈
- -enable-source-maps 에서 experimental 프리픽스 제거
[https://github.com/nodejs/node/pull/37362](https://github.com/nodejs/node/pull/37362)

## Deno

### [Deno 1.8 Released](https://deno.land/posts/v1.8)

- Deno 1.8 릴리즈
    - WebGPU 에 대한 실험적 지원
    - Intl API 빌트인 - 모든 JS Intl API 사용 가능
    - 프라이빗 모듈 fetch - 인증 토큰 지원
    - etc

### [Deno Websocket: A Simple WebSocket Library for Deno](https://github.com/ryo-ma/deno-websocket)

- deno 용 웹소켓 라이브러리. 노드의 ws

## GO

### [Putting Text on an Image with Go](https://josemyduarte.github.io/2021-02-28-quotes-on-images-with-go/)

- 이미지에 텍스트 삽입하기

## DB

### [How to Use a Machine Learning Model from a Google Sheet using BigQuery ML]()

## ETC

### [RFC 6455(WebSocket) Protocol](http://atug.kr/blog/archives/310)

- RFC 6455 웹소켓 프로토콜 번역본

# Javascript

### [jQuery 3.6.0 Released](http://blog.jquery.com/2021/03/02/jquery-3-6-0-released/)

- jsonp 오류에도 json return
- focus 시 실행하는 함수에서 다시 다른 엘리먼트를 focus할 때의 버그 수정
    - 마지막 포커스만 DOM 트리 위로 전파
- 3.0+ 버전에서 업그레이드할 때 호환성 문제 없도록 수정

### [V8 (and Chrome) to Get Faster Release Cycle](https://v8.dev/blog/faster-releases)

- V8, Chrome 의 릴리즈 주기를 6주에서 4주로 변경
- 내년(2022년)에는 크롬 100버전에 도달할 것으로 예상

### [Gatsby 3.0 Released](https://www.gatsbyjs.com/blog/gatsby-v3/)

- 로컬 개발 속도 향상(핫 리로드 속도 개선) - 사이트에서 변경된 부분만 빌드
- 더 빠른 빌드 시간(Incremental build) - 변경된 컨텐츠만 감지해서 업데이트
- web vitals, light house 개선 - [gatsby-plugin-image](https://www.gatsbyjs.com/docs/reference/built-in-components/gatsby-plugin-image/) 베타에서 일반으로 릴리즈
- 종속성 업데이트 - 노드12, 웹팩5, 리액트17, GraphQL15, ESLint7
- 개츠비 클라우드 - 개츠비 호스팅 공개

### [Electron 12.0.0 Released](https://www.electronjs.org/blog/electron-12-0)

- 크롬 89, 노드 14.16, V8 8.9 로 스택 변경

### QUICK BITS

[https://redmonk.com/sogrady/2021/03/01/language-rankings-1-21/](https://redmonk.com/sogrady/2021/03/01/language-rankings-1-21/)

- JS(1), Python(2), Java(3), PHP(4), CSS(5), Rust(19), Perl(19), Dart(21)

## Code & Tools

### [Shepherd: Guide Your Users Through a Tour of Your App](https://shepherdjs.dev/)

- 사이트에 튜토리얼을 넣게 해주는 서비스

### [web-minecraft: A Minecraft Client Written in JavaScript](https://github.com/michaljaz/web-minecraft)

- 웹 마인크래프트 - 반응이 좀 느림

### Quick release

[https://github.com/pixijs/pixi.js/releases/tag/v6.0.0](https://github.com/pixijs/pixi.js/releases/tag/v6.0.0) pixi js 6.0 릴리즈