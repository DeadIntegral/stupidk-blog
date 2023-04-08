---
title: dev-weekly 2023-02-04
date: "2023-02-04T12:20:00.000Z"
description: "dev-weekly 2023-02-04"
tags: ["javascript", "node", "css"]
---

# CSS

### **[CSS Art Tutorial: Create a Cute Cartoon Creature](https://blog.eleftheriabatsou.com/css-art-tutorial-create-a-cute-cartoon-creature)**

- CSS로 만화 캐릭터 그리기

### **[clamp() Calculator](https://chrisburnell.com/clamp-calculator)**

- min, max viewport와 폰트 사이즈를 입력하면 그에 상응하는 clamp를 만들어주는 계산기

### **[House Resizing with CSS Container Query](https://codepen.io/gayane-gasparyan/pen/yLqjVWb)**

- 리사이징하면 생김새가 바뀌는 집. only CSS

# Node

### **[Gatsby is joining Netlify](https://www.notion.so/2023-02-03-e4b57798c2654c8c8fcf12e2eb8c8e16)**

- Netlify에서 Gatsby 인수

### **[7 Awesome Free APIs for Your Next Node.js Project](https://maximorlov.com/awesome-apis-for-nodejs-projects/)**

- Nodejs 프로젝트를 위한 7가지 무료 API 서비스 소개

### **[TestCafe 2.3: Node-Based End-to-End Web Testing](https://github.com/DevExpress/testcafe/releases/tag/v2.3.0)**

- TestCafe 2.3릴리즈. 쉽게 셋팅할 수 있는 `create-testcafe` 커맨드 지원
- Node 14 지원 종료, 실험적인 ESM 지원

# Javascript

### **[You’ve Got Options for Removing Event Listeners](https://www.macarthur.me/posts/options-for-removing-event-listeners)**

- `.removeEventListener()`, `once` 등에 대한 설명
- `const { signal } = new AbortController()` 을 사용하여 event listener도 취소가능하고 여러 이벤트를 하나의 시그널로도 관리 가능

### **[Updates from the 94th TC39 meeting](https://dev.to/hemanth/updates-from-the-94th-tc39-meeting-48mb)**

- Stage4 - Change Array by Copy, Intl.NumberFormat V3, Symols as WeekMap keys
- Import Assertion은 스테이지3에서 2로 격하

### **[You May Not Need Lodash or Underscore](https://github.com/you-dont-need/You-Dont-Need-Lodash-Underscore#readme)**

- You May Not JQuery에서 영감을 받은 유틸 라이브러리 스니펫 모음
- You Dont Need 시리즈

### **[The Future of *Create React App* and Why It Exists](https://github.com/reactjs/reactjs.org/pull/5487#issuecomment-1409720741)**

- Dan이 작성한 CRA의 배경 및 상태, 추구하는 방향, React 와 framework간의 관게
- 결론: CRA를 런처로 전환하는 방향으로 기우는 중.

### **[FeedbackPlus: Add Screenshot Tools to Your Feedback Forms](https://github.com/ColonelParrot/feedbackplus)**

- 현재 화면을 캡쳐하고, 수정할 수 있는 피드백 폼을 제공하는 라이브러리

### **[Swiper 9.0: Mobile Touch Slider with Accelerated Transitions](https://github.com/nolimits4web/swiper/releases/tag/v9.0.0)**

- Swiper 9.0 릴리즈
- 새로운 Swiper Element(웹 컴포넌트) - Solid, Angular, Svelte 컴포넌트 제거
- Zoom, Virtual Slide등 다양한 기능 제공

### **[UUID.js: RFC-Compliant UUID Generator](https://github.com/LiosK/UUID.js)**

- RFC를 준수한 UUID v1~v4 생성기

### Release

- **[Nest 9.3](https://github.com/nestjs/nest/releases) -** Nest 9.3 릴리즈(글 작성 시점에 9.3.2)
- **[Docusaurus 2.3](https://github.com/facebook/docusaurus/releases/tag/v2.3.0)** - Docusaurus 2.3 릴리즈 (글 작성 시점에 2.3.1)
- **[Electron 22](https://github.com/electron/electron/releases/tag/v22.0.0)** - 일렉트론 22 릴리즈 (글 작성 시점에 22.2.0)
- **[Jotai 2.0](https://github.com/pmndrs/jotai/releases/tag/v2.0.0)** - Jotai 2.0 릴리즈. 마이그레이션 가이드 제공
- **[ReScript 10.1](https://rescript-lang.org/blog/release-10-1)** - 새로운 Await, async, Promise, JSX v4 신택스
- [madge 6.0](https://github.com/pahen/madge/releases/tag/v6.0.0)

# ETC

### **[Go 1.20 Released](https://go.dev/blog/go1.20)**

- PGO(Profile-guided optimizion) 앱의 프로필 실행을 사용하는 컴파일 최적화
- GC 성능 향상, Error는 다른 error들을 래핑 가능
- 윈도7,8 및 맥 10.13,10.14 를 지원하는 마지막 릴리즈