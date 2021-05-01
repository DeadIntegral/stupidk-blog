---
title: dev-weekly 2021-05-01
date: "2021-05-01T09:40:00.000Z"
description: "dev-weekly 2021-05-01"
tags: ["javascript", "css", "db"]
---

# CSS, DB

## CSS

### [The Almost-Complete Guide to Cumulative Layout Shift](https://jessbpeck.com/posts/completecls/)

- CLS(Cumulative Layout Shift)에 대한 가이드

## DB

### [Getting Into Y Combinator with a Fork of Redis](https://console.dev/qa/keydb-john-sully/)

- KeyDB는 Redis의 멀티 스레드 포크
- KeyDB 제작자와의 인터뷰

# Javascript

### [Babel 7.14.0 Released](https://babeljs.io/blog/2021/04/29/7.14.0)

- Class fields 와 private methods 디폴트 활성화
- importInterop: node 를 통한 듀얼 모듈
- 타입스크립트 4.3 지원
- async do expresstion 지원 (stage1)

### [Redux 4.1 Released](https://github.com/reduxjs/redux/releases/tag/v4.1.0)

- 번들크기 감소(2.6kb ⇒ 1.6kb gz)
- 프로덕션 모드에서 오류 메시지 추출(extract)
- RTK 에 rtk-query 병합 알파
    - [https://github.com/reduxjs/redux-toolkit/releases/tag/v1.6.0-alpha.1](https://github.com/reduxjs/redux-toolkit/releases/tag/v1.6.0-alpha.1)

Quick Bits

- [https://www.zdnet.com/article/programming-languages-javascript-has-most-developers-but-rust-is-the-fastest-growing/](https://www.zdnet.com/article/programming-languages-javascript-has-most-developers-but-rust-is-the-fastest-growing/) 개발자 생태계 크기
    - [https://www.zdnet.com/article/the-rust-programming-language-just-took-a-huge-step-forwards/](https://www.zdnet.com/article/the-rust-programming-language-just-took-a-huge-step-forwards/) 러스트 파운데이션 설립
- [https://github.com/angular/angular/issues/41840](https://github.com/angular/angular/issues/41840) 앵귤러도 뷰3와 마찬가지로 ie11 지원 중단
- [https://wicg.github.io/sanitizer-api/](https://wicg.github.io/sanitizer-api/) 신뢰할 수 없는 문자열을 제거하기 위해 제안된 API

## Articles, Opinions & Tutorials

### [Using Asynchronous Web APIs from WebAssembly](https://web.dev/asyncify/)

- Asyncify 를 이용하여 동기식 언어의 API 를 WASM으로 컴파일 할 때 비동기로 만들기

## Code & Tools

### [Scribbletune 4.0: Use Strings and Arrays to Create Rhythms and Musical Patterns](https://github.com/scribbletune/scribbletune)

- JS로 음악 만들기 - MIDI 파일로 export 가능

### [js-tokens 7.0: A Tiny JavaScript Tokenizer](https://github.com/lydell/js-tokens)

- Tiny JavaScript tokenizer. 벤치마크로는 `@babel/parser` 보다 월등한 성능