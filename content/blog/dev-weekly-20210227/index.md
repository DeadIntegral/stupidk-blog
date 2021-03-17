---
title: dev-weekly 2021-02-27
date: "2021-02-27T08:30:00.000Z"
description: "dev-weekly 2021-02-27"
tags: ["javascript", "css", "node", "web", "DB"]
---

# CSS, Node, DB, ETC

## CSS

### [Building a Tabs Component](https://web.dev/building-a-tabs-component)

- 마치 모바일처럼 탭 클릭 시 스크롤이 움직이듯 화면이 전환하는 방법

### [Diving Into the ::before and ::after Pseudo-Elements](https://codersblock.com/blog/diving-into-the-before-and-after-pseudo-elements/)

- 라인, 리본, block-quote 등의 UI 예제
- counter, @property 등 draft 기술들 예제

### [Use CSS Variables instead of React Context](https://epicreact.dev/css-variables)

- 테마를 설정할 때 react context 대신(css in js의 ThemeProvider) css variable을 쓰는게 좋은 이유
- Kent C.Dodds 의 글

<hr />

## Node

### [Tauri: A New(ish) Framework for Building Desktop Apps with a Web Frontend](https://tauri.studio/en/)

- 일렉트론과 같은 데스크탑 앱 빌드 도구.
- 러스트로 제작

[Working with Protobufs in Node]()

- nodejs에서 protobuf 사용하기

[Tree-Sitter: A Parser Generator Tool and Incremental Parsing Library](https://tree-sitter.github.io/tree-sitter/)

- rust로 작성된 incremental parsing system
- nodejs 및 wasm binding 존재

### [ZWS: A URL Shortener Based on Invisible Spaces](https://github.com/zws-im/zws)

- 보이지 않는 공백문자를 이용해서, url을 짧게 보이게 하는 서비스(항상 [zws.im](http://zws.im) 으로 보임)
- 절대 권장하진 않지만, funny + clever

<hr />

## DB

### [Read Consistency with Database Replicas at Shopify](https://shopify.engineering/read-consistency-database-replicas)

- 읽기 전용 레플리카를 사용할 때 복제 지연에 대한 shopify의 후기
- 세 가지 솔루션
    - Tight Consistency
    - Causal Consistency - [https://jepsen.io/consistency/models/causal](https://jepsen.io/consistency/models/causal)
    - Read Consistency(shoptify의 솔루션) - [https://jepsen.io/consistency/models/monotonic-reads](https://jepsen.io/consistency/models/monotonic-reads)

### [29 Bite-Sized DynamoDB Best Practices](https://dynobase.dev/dynamodb-best-practices/)

- 다이나모 디비의 모델링, 보안, 성능, 설계에 대한 짧은 팁들 모음

<hr />

## ETC

[https://userguiding.com/blog/ux-ui-trends/](https://userguiding.com/blog/ux-ui-trends/)

<hr />

# Javascript

### [JavaScript Performance Beyond Bundle Size](https://nolanlawson.com/2021/02/23/javascript-performance-beyond-bundle-size/)

- 요즘 번들 사이즈에 초점이 맞춰져 있는데, 번들 사이즈도 중요하지만 parse/compile time, excutution time, power, memory, disk usage도 중요하다는 글
- 각 항목을 어떻게 측정하는지 설명

### [The Definitive Guide to Streams](https://web.dev/streams/)

- 스트림에 관련된 용어설명부터, 어떻게 사용하는지까지 자세한 설명

### [TypeScript 4.2 Released](https://devblogs.microsoft.com/typescript/announcing-typescript-4-2/)

- TS 4.2 릴리즈

## [10 Years of Open-Source Visualization with D3.js](https://observablehq.com/@mbostock/10-years-of-open-source-visualization)

- d3 제작자분의 1.0 릴리즈 이후 지난 10년간의 후기
- 오픈소스에 대한 마음가짐 및 방향성

### Quick Bits

[https://free-for.dev/#/](https://free-for.dev/#/)

- 개발자를 위한 프리 티어 서비스 모음(free trial 제외)
- 프리티어는 기간제일 경우 1년 이상 제공해야 하고, tls를 유료로 제공하는 서비스는 제외

[https://storybook.js.org/blog/storybook-vue3/](https://storybook.js.org/blog/storybook-vue3/)

- 스토리북에서 vue3 공식지원

<hr />

## Code & Tools

### [Simple-Keyboard: A Virtual Keyboard for JavaScript Projects](https://virtual-keyboard.js.org/)

- 커스터마이징 가능하고, 가볍고, 바닐라 및 리앵뷰에 호환되는 가상키보드

### [Tagger: A Zero Dependency, Vanilla JavaScript Tagging Library](https://github.com/jcubic/tagger)

- 태그 에디터

### Quick release

[https://github.com/puppeteer/puppeteer/releases/tag/v8.0.0](https://github.com/puppeteer/puppeteer/releases/tag/v8.0.0)

- 퍼펫티어 8.0 릴리즈

[https://github.com/addyosmani/critical/releases/tag/v3.0.0](https://github.com/addyosmani/critical/releases/tag/v3.0.0)

- addy osmani 의 라이브러리 critical 3.0 릴리즈
- critical path 를 추출하는 라이브러리