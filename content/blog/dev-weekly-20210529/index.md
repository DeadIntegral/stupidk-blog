---
title: dev-weekly 2021-05-29
date: "2021-05-29T09:30:00.000Z"
description: "dev-weekly 2021-05-29"
tags: ["javascript", "css", "node"]
---

# CSS

## CSS

### [Learn CSS](https://web.dev/learn/css)

- 웹 스타일링 전문 지식 함양을 위한 참고 자료

### [Making Disabled Buttons More Inclusive](https://css-tricks.com/making-disabled-buttons-more-inclusive)

- 비활성화 버튼 disable 하면 tab으로 선택이 안됨(웹 접근성 이슈)
- 대신 aria-disabled=true를 하는것이 좀 더 나은선택
- 그리고 보다 더 나은 케이스

---

## Node

### [Express 5.0 alpha](https://expressjs.com/en/5x/api.html)

- [https://github.com/expressjs/express/blob/5.0/History.md](https://github.com/expressjs/express/blob/5.0/History.md)

### [A Deep Dive into Rust for Node Developers](https://itnext.io/deep-dive-into-rust-for-node-js-developers-5faace6dc71f)

- 노드 개발자를 위한 rust deep dive
- [https://play.rust-lang.org/?version=nightly&mode=debug&edition=2018](https://play.rust-lang.org/?version=nightly&mode=debug&edition=2018)

### [node-notifier 10.0: Cross Platform Native Notifications from Node](https://github.com/mikaelbr/node-notifier)

- native notifications 모듈. 일렉트론 호환
- 맥, 윈도, 리눅스 등 지원하는 크로스 플랫폼

---

# Javascript

### [Sparkplug: V8's Non-Optimizing JavaScript Compiler](https://v8.dev/blog/sparkplug)

- 인터프리터는 매우 빠르지만 `바이트코드 디코딩`이나 `디스패치` 와 같은 제거할 수 없는 오버헤드를 갖고 있음
- ignition 인터프리터와 turbopan 컴파일러 사이 계층
- 사실 Sparklug는 내장 된 호출 및 제어 흐름 코드. 인터프리터 실행의 직렬화. 그러나 위의 제거불가능한 오버헤드를 제거(pre-compile)

### [TypeScript 4.3 Released](https://devblogs.microsoft.com/typescript/announcing-typescript-4-3/)

### [Jest 27 Released, Complete with Some New Defaults](https://jestjs.io/blog/2021/05/25/jest-27)

- interactive 모드를 사용하여 실패한 테스트를 하나씩 단계별 실행
- 기본값 변경
    - 테스트 환경 변경 기능 - jsdom, node `"testEnvironment": "jsdom`
    - 타이머 변경 `jest.useFakeTimers("legacy")` , `"timers": "legacy"`

---

## Quick Byte

### 앵귤러의 새로운 기능 요청 프로세스

- [https://blog.angular.io/new-feature-request-process-a9f69d106fc8](https://blog.angular.io/new-feature-request-process-a9f69d106fc8)
- 티켓을 받으면 앵귤러 팀원이 수동으로 검토하고 기능 요청 혹은 문제로 분류
- 기존 로드맵의 프로젝트와 일치하는지 확인하여 우선순위 지정, 그렇지 않으면 60일의 투표 기간
- 20표 이상의 요청을 고려

### Flow 여전히 오픈소스 유지하지만, 페이스북 사용 사례에 맞춰 개발하기로 변경

- [https://medium.com/flow-type/clarity-on-flows-direction-and-open-source-engagement-e721a4eb4d8b](https://medium.com/flow-type/clarity-on-flows-direction-and-open-source-engagement-e721a4eb4d8b)

---

## Articles, Opinions & Tutorials

### [New Standards to Access User Device Hardware from JavaScript](https://blog.bitsrc.io/new-standards-to-access-user-device-hardware-using-javascript-86b0c156dd3d)

- WebHID - 한 번에 하나의 기기만 연결 가능
- WebNFC - 안드로이드 크롬만 지원, https 하에서만 허용
- WebUSD - 드라이버가 필요하지 않음

### [Get Started with React by Building a 'Whac-a-Mole' Game](https://www.smashingmagazine.com/2021/05/get-started-whac-a-mole-react-game/)

- 리액트로 두더지 게임 만들기
- 프로그램을 어떻게 만들어야 하는지 사고방식에 대한 예시.

### [Where's The Best Place to Host a Next.js Site?](https://kontent.ai/blog/comparison-of-jamstack-hosting-platforms-for-next-js)

- Nextjs 호스팅을 위해 vercel, netlify, heroku, layer0 비교
- 비교항목
    - 깃헙 연동
    - 푸시했을 때 자동 빌드
    - 컨텐츠 변경 시 자동 빌드
    - 성능(빌드 시간)
    - 추가 기능(analytics 등)
    - 가격 및 프리티어 제한

---

## Code & Tools

### [threads.js: Web Workers Meet Worker Threads](https://threads.js.org/)

- [https://github.com/andywer/threads.js](https://github.com/andywer/threads.js)
- 웹 워커와 워커 스레드를 함수 호출 형태로 사용하게 해주는 도구