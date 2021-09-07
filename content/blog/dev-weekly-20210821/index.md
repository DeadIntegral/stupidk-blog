---
title: dev-weekly 2021-08-21
date: "2021-08-21T09:00:00.000Z"
description: "dev-weekly 2021-08-21"
tags: ["javascript", "css"]
---


# CSS

### [Building a Switch Component](https://web.dev/building-a-switch-component)

- 스위치 컴포넌트 만들기 feat.접근성 및 애니메이션

### [Accessible Overflow](https://marcus.io/blog/accessible-overflow)

- 스크린 리더기 등에서는 화살표 키를 이용해 스크롤을 하는데, 이 때에 포커스가 특정 컨테이너가 아니라 문서 전체가 될 수 있음
- 특정 컨테이너에 포커스 주기
- role, aria-label, tabindex

### [Tunnel Travel Using CSS Perspective](https://codepen.io/trangthule/pen/vYmpNYR)

- CSS Only - 이미지 사용

# Javascript

### [Ruby on Rails' Creator on Modern Web Apps without JS Bundling or Transpiling](https://world.hey.com/dhh/modern-web-apps-without-javascript-bundling-or-transpiling-a20f2755)

- 루비 온 레일즈 창시자가 rails 기반 앱에서의 JS방향에 대해 말하는 글
- ES6, HTTP2(Bundler out), Import (ESM)

### [Announcing React Native 0.65](https://reactnative.dev/blog/2021/08/17/version-065)

- RN 0.65 릴리즈
- Hermes 0.8.1 업그레이드
- 접근성

### [Map overflow](https://searchvoidstar.tumblr.com/post/659634228574715904/an-amazing-error-message-if-you-put-more-than-2-24)

- Map 객체에 키를 스트링으로 넣으면 2^24 에서 오버플로우
- 작동 원리(버그가 아닌 기능) - [https://stackoverflow.com/questions/54452896/maximum-number-of-entries-in-node-js-map](https://stackoverflow.com/questions/54452896/maximum-number-of-entries-in-node-js-map)
- 숫자를 넣으면 억단위에서 Uncaught RangeError: Invalid array length at

### [How to Write TypeScript Interfaces in JSDoc Comments](https://goulet.dev/posts/how-to-write-ts-interfaces-in-jsdoc/)

- jsDoc Comment를 이용하여 TS Interface를 작성하는 방법
    - TS Build를 하지 않고 TS 타입만 사용하기

### [Marked 3.0: A Fast Markdown Parser and Compiler](https://github.com/markedjs/marked/releases/tag/v3.0.0)

- marked 3.0 릴리즈
- [https://marked.js.org/demo/](https://marked.js.org/demo/) 데모

### [Notistack: A Library for Easy Snackbar/Toast Notifications](https://github.com/iamhosseindhv/notistack)

- 커스텀 가능한 알림 스낵바(토스트)
- redux/mobx 지원