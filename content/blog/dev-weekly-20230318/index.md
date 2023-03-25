---
title: dev-weekly 2023-03-18
date: "2023-03-18T12:40:00.000Z"
description: "dev-weekly 2023-03-18"
tags: ["javascript", "css", "node"]
---

# CSS

### **[Ten Tips for Better CSS Transitions and Animations](https://joshcollinsworth.com/blog/great-transitions)**

- CSS Transition, Animation을 더 잘 만들기 위한 팁들
- 애니메이션 중 요소가 많이 변경되면 전환이 과도해 보일 수 있음
- 브라우저 내장 곡선(ease, ease-in, ease-out, ease-in-out 등)을 피하고 cubic-bezier 곡선 사용하기 (VSCode 내장이 있어서 자동 완성 제공)

# Node

### **[Shell-Free Scripts with Execa 7.1](https://itnext.io/shell-free-scripts-with-execa-7-885fb3b42f83)**

- shell 없이 스크립트 만들기 - 컨셉 및 예제
- 모든 명령에 대해 모든 플랫폼의 쉘을 만드는 것은 비용인데 Execa 는 로컬에 설치된 바이너리를 직접 실행

### **[10 years of Electron](https://www.electronjs.org/blog/10-years-of-electron)**

- 일렉트론의 10번째 생일 (2013년 3월 13일 첫 커밋) 을 맞이하여 회고
- atom shell로 시작했으나 이후 Electron으로 이름 변경. 거버넌스 모델로 전환할즈음 Electron 소유권을 Github에서 OpenJS 재단으로 이전.
- 컴파일, 인증, 권한 관리 등 다양한 영역을 자동화 해온 과정 소개

### **[How to Debug Node Segmentation Faults](https://httptoolkit.com/blog/how-to-debug-node-segfaults/)**

- Segmentation fault 에 대한 소개 및 발생 원인
    - 잘못된 메모리 주소 읽기쓰기, Stack(Buffer) over flow, 내 것이 아닌 메모리 읽기쓰기 등
- 포인터, 메모리 이슈 등은 로우 레벨이라 JS는 발생하지 않지만, Node에서 Seg fault 가 발생하는 경우
    - 네이티브 에드온에서 발생, 노드 객체의 내부 비공개 상태를 조작하는 경우, NodeJS 자체 버그 등

### **[Introducing Mongoose 7: The MongoDB ODM for Node](https://thecodebarbarian.com/introducing-mongoose-7.html)**

- Mongoose 7.0 릴리즈.
- 콜백 제거 - 콜백을 한 번도 사용해본 적 없는 세대의 등장.
- strictQuery false를 기본값으로 복원, orFail, updateOne, add 등 새로운 기능들 추가

### **[Find My Way: Fast HTTP Router That Uses Radix Trees](https://github.com/delvedor/find-my-way)**

- 내부적으로 Radix tree를 사용했고 프레임워크와 독립적인 매우 빠른 http router

# Javascript

### **[Transformers.js: Running ML Models in the Browser](https://xenova.github.io/transformers.js/)**

- 자연어 처리, 시각 처리에 주로 사용되는 ML 모델의 일종. 브라우저에서 실행하게 해주는 도구

### **[Announcing TypeScript 5.0](https://devblogs.microsoft.com/typescript/announcing-typescript-5-0/)**

- TS 5.0 릴리즈
- RC, 베타와 차이점
    - export 전후에 데코레이터 배치
    - 새로운 번들러 모듈 레졸루션 옵션은 —module 이 esnext로 설정된 경우만 사용 가능
    - package.json에서 nodejs 최소 12.20 지정

### **[Chrome 111 Gains a 'View Transition' Feature for SPAs](https://developer.chrome.com/blog/spa-view-transitions-land/)**

- 페이지 전환 애니메이션 view transition 크롬 111에 추가 (현재 플래그 활성화 필요)
- 아직 다른 브라우저는 지원할지 알 수 없으나 점진적 향상 기법으로 도입 가능
- same origin에서 작동하고 meta tag에서 제어중이지만 CSS로 전환할 수 있음

### JS Library Chore

**[React ProseMirror: Integrate the ProseMirror Editor with React](https://github.com/nytimes/react-prosemirror)**

- React와 ProseMirror 통합하는 라이브러리. useEditorEffect, useEditorEvent 등 제공

**[Recharts 2.5](https://github.com/recharts/recharts/releases/tag/v2.5.0)**

- Rechart 2.5 릴리즈

# ETC

### **[Design First, Then Build”: Let’s Bury This Myth Forevermore](https://evilmartians.com/chronicles/design-first-then-build-lets-bury-this-myth-forevermore)**

- 디자인 후 개발에 대한 대안
    - Mantra 1. 지금 당장 필요한 것만 디자인하기
    - Mantra 2. 디자인 즉시 구현 - 제품이 복잡해지면 추적해야 할 맥락이 복잡해짐
    - Mantra 3. 디자인 단계에서 큰 기능을 작은 작업으로 나누기
    - Mantra 4. 디자인과 개발간 커뮤니케이션 체계화

### **[The first version of your favorite digital products.](https://www.theversionone.com/)**

- 유명한 제품들(스포티파이, 트위터, 에이비앤비, 왓츠앱, 슬랙, 깃헙, 링크드인, 넷플릭스 등)의 초기 버전 UI 모음 서비스