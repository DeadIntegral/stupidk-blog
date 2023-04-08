---
title: dev-weekly 2023-01-21
date: "2023-01-21T15:20:00.000Z"
description: "dev-weekly 2023-01-21"
tags: ["javascript", "node", "css"]
---
# CSS

### **[Conditional CSS](https://ishadeed.com/article/conditional-css)**

- CSS의 조건부 설계 및 예제
    - MediaQuery - CSS Conditional Rules Module
    - gap, flex-grow, flex-basis 와 같은 암시적인 조건
- [조건부 border-radius](https://ishadeed.com/article/conditional-border-radius/)
    
    ```css
    .card {
      border-radius: max(
        0px,
        min(8px, calc((100vw - 4px - 100%) * 9999))
      );
    }
    ```
    

### **[CSS Style Queries](https://ishadeed.com/article/css-container-style-queries)**

- 컨테이너의 CSS property, variable을 쿼리
- `@container style(display: flex)` , `@container stats style(--theme: dark) {` 와 같은 방법을 통해 중첩되어야 하는 css를 플랫하게 변경 가능하고, 배리언트 대체 가능

# Node

### **[Bun v0.5 Released](https://bun.sh/blog/bun-v0.5.0)**

- Bun.dns, Node.dns, node:tls, node:net, node:readline 등 지원
- bun:test 향상, 성능 향상
- module resolution 변경

### **[Blue Green Deployment for Node.js without Kubernetes](https://semaphoreci.com/blog/blue-green-deployment-nodejs)**

- 쿠버네티스 없이 nodejs 블루 그린 배포하기
- nginx, pm2를 활용하여 블루그린배포

### **[Blockman: Highlight Nested Code Blocks in VS Code](https://marketplace.visualstudio.com/items?itemName=leodevbro.blockman#blockman)**

- 블록에 border를 그려서 현재 작업중인 영역을 강조해주는 vscode 플러그인

# Javascript

### **[The WebAssembly JavaScript Promise Integration API](https://v8.dev/blog/jspi)**

- 동기식 API를  호출 할 때 애플리케이션을 일시 중단하고, 비동기 작업이 완료되면 다시 시작
- WASM 앱이 외부 기능에 대한 동기/비동기 간극을 줄이는 API

### **[Why Is My Jest Suite So Slow?](https://blog.bitsrc.io/why-is-my-jest-suite-so-slow-2a4859bb9ac0)**

- 유닛 테스트 시간과 제스트 실행 시간이 일치하지 않는 이유
- 시작시간 - 약 1초 소요, 우리 앱과 독립적이고 스레드 당 한번 발생하고 확장되지 않음
- 캐시 채우기 - 첫 실행 시간의 대부분은 TS 변환시간.
- 테스트 파일 로드 - 대부분의 시간 소모. Barrel File 이슈
    - Jest는 우리가 가져오는 컴포넌트가 어디 있는지 모르고, 때문에 전체 파일을 로드하느라 시간 소모 ⇒ 경로를 정확하게 명시해주면 해결
- 테스트 실행에서 타입 검사 제거 - TS 컴파일러가 하는 일 중복
- 전체 테스트 실행하지 않기 - Jest는 변경된 파일을 기반으로 실행해야 하는 하위집합을 파악할 수 있음

### **Release**

- **[Remix 1.10.0](https://github.com/remix-run/remix/releases/tag/remix%401.10.0)**
- [axios 1.2.3](https://github.com/axios/axios/releases/tag/v1.2.3)
- [esbuild 0.17](https://github.com/evanw/esbuild/releases/tag/v0.17.0) - 글 작성 시점엔 0.17.3
- **[React Native 0.71](https://reactnative.dev/blog/2023/01/12/version-071)**

### **[Handling Errors Like a Pro in TypeScript](https://engineering.udacity.com/handling-errors-like-a-pro-in-typescript-d7a314ad4991)**

- 커스텀 오류 타입 만들기

### **[RoughNotation: Cute Animated 'Rough' Text Annotations](https://roughnotation.com/)**

- DOM을 선택하면 해당 영역에 손으로 그린듯한 강조 표시를 애니메이션 해주는 도구

### **[gpu-io: GPU-Accelerated Computing Library](https://github.com/amandaghassaei/gpu-io)**

- 물리 시뮬레이션, 수학 계산을 위한 GPU 가속 라이브러리