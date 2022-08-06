---
title: dev-weekly 2022-08-06
date: "2022-08-06T08:00:00.000Z"
description: "dev-weekly 2022-08-06"
tags: ["javascript", "node", "css"]
---

# CSS

### **[Finer Grained Control Over CSS Transforms With Individual Transform Properties](https://web.dev/css-individual-transform-properties/)**

- transform에 여러 값을 입력 후 하나의 값을 변경하려면 모든 값을 복사 후 하나의 값을 변경해야했음
- 크롬104에서 개별 transform을 지원하면서 transform의 각 프로퍼티를 나눠서 입력 가능
- 한번에 입력할 땐 왼쪽 ⇒ 오른쪽 순서 적용이지만, 개별 프로퍼티는 translate, rotate, scale 순(외부에서 내부)

### **[Recreating MDN’s Truncated Text Effect](https://css-tricks.com/recreating-mdns-truncated-text-effect)**

- text-overflow: ellipsis 는 뒷 부분의 글자가 잘림
- 전체 텍스트를 입력 후 css effect를 주고 스크린 리더기는 전체 텍스트를 읽게 하는 방법

### **[axe Accessibility Linter for VSCode](https://marketplace.visualstudio.com/items?itemName=deque-systems.vscode-axe-linter)**

- 리액트, 뷰, 앵귤러에서 접근성 린팅을 해주는 익스텐션. 제로 컨피그

# Node

### **[Introducing the New npm Dependency Selector Syntax](https://github.blog/changelog/2022-08-03-introducing-the-new-npm-dependency-selector-syntax/)**

- `npm query` - npm 8.16.0 에서 추가된 기능
- css query selector와 유사한 방식으로 의존성 검색
- ex) `npm query "*"` (npm list —all) , `npm query "[license=MIT]"` 등

### **[Electron 20 Released: The Cross Platform Desktop App Platform](https://www.electronjs.org/blog/electron-20-0)**

- 크롬104, V8 10.4, 노드 16.15 포함
- UI 수정 및 V8 샌드박스 포인터 활성화

### **[A DIY `node_modules` Cache for Docker in Your CI](https://remelehane.dev/posts/diy-node-cache-for-docker-ci/)**

- 빌드 성능을 향상시키기 위한 아이디어 - 노드 캐시 이미지(컨테이너)를 만들고, 캐시 이미지를 사용하여 이미지를 만드는 방법
- 캐시 이미지는 주기적으로 새로 빌드

# Javascript

### **[JS1024 2022 Competition Winners](https://js1024.fun/results/2022)**

- 1024바이트 대회 2022년 결과(프로젝트 모음)

### **[Docusaurus 2.0 Released](https://docusaurus.io/ko/blog/2022/08/01/announcing-docusaurus-2.0)**

- 정적 사이트 생성도구 Docusaurus 2.0 발표 (4년전부터 2 이용이 가능했지만 시멘틱 버저닝 때문에)

### **[a multiplayer game in Word](https://www.youtube.com/watch?v=87nzxrRFq8U)**

- MS워드를 캔버스로 멀티플레이어 게임 제작(스트리트 파이터)

### [VSCode **1.70 Release**](https://code.visualstudio.com/updates/v1_70)

- [https://twitter.com/stefanjudis/status/1555466217774882818](https://twitter.com/stefanjudis/status/1555466217774882818) sticky scrolling 기능
- 터미널 렌더링 향상

# Go

### **[Go 1.19 Released](https://go.dev/blog/go1.19)**

- Go의 메모리 모델은 이제 sync/atomic 패키지의 동작을 명시적으로 정의
- 보안상의 이유로 os/exec 패키지는 path 조회에서 상대경로 고려 안함
- 가비지 콜렉터는 소프트 메모리 제한에 대한 지원 추가