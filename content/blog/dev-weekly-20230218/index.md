---
title: dev-weekly 2023-02-18
date: "2023-02-18T12:40:00.000Z"
description: "dev-weekly 2023-02-18"
tags: ["javascript", "css", "node"]
---
# CSS

### **[Moving Backgrounds](https://css-tricks.com/moving-backgrounds)**

- 제한된 영역 내에서 커서의 위치에 따라 배경이 움직여 보다 큰 이미지를 보여주는 코드(ex 커머스)
- 커서에 hover된 영역만큼 돋보기 효과 주기

### **[Different Ways to Get CSS Gradient Shadows](https://css-tricks.com/different-ways-to-get-css-gradient-shadows)**

- box-shadow대신 Gradient로 그림자 만들기
- stacking context 해결하기, 투명도를 지원하는 gradient shadow, border-radius에 맞춰서 그림자 설정하기

# Node

### **[How To Scale Node Apps with Clustering](https://www.digitalocean.com/community/tutorials/how-to-scale-node-js-applications-with-clustering)**

- NodeJS 클러스터링을 통한 확장
- 노드가 갖고 있는 기본적인 컨셉에서부터 잘 설명해주는 튜토리얼 문서

### **[Pythagora: Generate Integration Tests by Recording App Activity](https://github.com/Pythagora-io/pythagora)**

- 앱에 통합되어 코드 한줄을 추가하면 앱의 사용량을 캡쳐하고 통합 테스트를 만들어주는 도구

### **[WebContainer API is here.](https://blog.stackblitz.com/posts/webcontainer-api-is-here/)**

- Public WebContainer API 출시
- web VSCode인 Codeflow IDE가 웹 컨테이너 제품

### **[Execa 7.0: A Better child_process](https://github.com/sindresorhus/execa)**

- child_process 보다 많은 정보를 인간을 위해 표기해주는 도구 Execa 7.0 릴리즈 (노드 14이상 지원)

# Javascript

### **[Ryan Dahl, Node.js Creator, Wants to Rebuild the Runtime of the Web](https://www.sequoiacap.com/article/deno-spotlight/)**

- NodeJS 창시자 라이언 달의 일대기
- nodejs에서 마주친 상황들, 딥브레인에서 deeplearn.js, deno에 이르기까지

### **[Angular Reactivity with Signals](https://github.com/angular/angular/discussions/49090)**

- 앵귤러에 solidjs, Preact 등에서 사용중인 Signals 도입

### **[Web Push for Web Apps on iOS and iPadOS](https://webkit.org/blog/13878/web-push-for-web-apps-on-ios-and-ipados/)**

- Safari 16.4에서 Web Push 지원

### **[why `a = 0-x` is about 3-10x faster than `a = -x`](https://twitter.com/mhevery/status/1626002464469323777)**

- a = -x 보다 a = 0 - x가 3~10배 빠른 이유를 설명하는 트윗
- JS의 숫자는 Int와 Float로 나뉘어져 있고, Int는 -0을 가질 수 없음. 배열에 넣을 경우 배열에 int, float가 섞여있어서 컨버팅 과정이 추가

### **[Mermaid 9.4](https://github.com/mermaid-js/mermaid/releases/tag/v9.4.0)**

- mermaid 9.4 릴리즈. 타임라인 포맷 지원.

### **[Use a MutationObserver to Handle DOM Nodes that Don’t Exist Yet](https://www.macarthur.me/posts/use-mutation-observer-to-handle-nodes-that-dont-exist-yet)**

- 아직 존재하지 않는 DOM Node를 컨트롤할 때 뮤테이션 옵저버 사용하기
- 과거에 사용했던 폴링 등 보다 성능이 좋음. 구글 리캡차를 완료했을 때 감지하기 등의 예제

### **[Use a MutationObserver to Handle DOM Nodes that Don’t Exist Yet](https://h3manth.com/posts/Well-known-symbols/)**

- 잘 알려진 JS Symbol이 어떤 일을 하는지 설명하는 TC39의 대표 Hemanth의 글
- 14가지 심볼 소개
    - iterator - for of, spread 등을 사용한 루프 활성화
    - toStringTag - Object.prototype.toString 가 반환하는 값 지정

### **[Dependency Cruiser: Validate and Visualize JavaScript Dependencies](https://github.com/sverweij/dependency-cruiser)**

- 의존성 변경(코드 변경 시 영향을 받는 곳)에 대한 시각화를 제공하는 도구

### **[NodeGUI: Build Native Cross-Platform Desktop Apps with Node.js](https://github.com/nodegui/nodegui/releases/tag/v0.58.0)**

- NodeGUI 0.58 릴리즈. Qt6을 기반으로 하는 NodeGUI의 첫 번째 안정적인 릴리즈.

### **[DOMPurify 3.0: Fast, Tolerant XSS Sanitizer for HTML and SVG](https://github.com/cure53/DOMPurify/releases/tag/3.0.0)**

- html, svg 를 넣으면 XSS로부터 안전한 코드로 반환하는 도구 DOMPurify 3.0 릴리즈