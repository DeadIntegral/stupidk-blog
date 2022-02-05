---
title: dev-weekly 2022-02-05
date: "2022-02-05T08:30:00.000Z"
description: "dev-weekly 2022-02-05"
tags: ["javascript", "css", "node", "web", "DB"]
---

# CSS

### **[Fancy CSS Borders Using Masks](https://css-tricks.com/css-borders-using-masks)**

- CSS 마스크를 이용한 테두리 꾸미기 (약간의 계산)
- 만들어주는 생성기 [https://css-generators.com/custom-borders/](https://css-generators.com/custom-borders/)

### **[Here’s What I Didn’t Know About :where()](https://www.matuzo.at/blog/2022/heres-what-i-didnt-know-about-where)**

- `:where()` 를 사용하여 specificity 낮추기

# Node

### **[The Fetch API Comes to Node Core (and Why You Should Care)](https://fusebit.io/blog/node-fetch/)**

- Node18부터 fetch API 코어에서 지원
- fetch에 대한 간략한 설명

### **['How I Reversed a Node.js Malware and Found The Author'](https://itnext.io/how-i-reversed-a-nodejs-malware-and-found-the-author-7dd9531b389f)**

- 디스코드 서버에 올라온 악성파일을 리버시 엔지니어링하고 제작자를 찾은 과정

### **[Top 100 npm Package Maintainers Now Must Use 2FA](https://github.blog/2022-02-01-top-100-npm-package-maintainers-require-2fa-additional-security/)**

- 주간 다운로드 100만건 이상, 혹은 500건 이상의 종속성이 있으면 2FA 필수
- 2022년 2월1일부터 npm 상위 100개 패키지는 2FA 필수
    - 2FA비활성화 메인테이너는 세션 취소

### **[V8 release v9.9](https://v8.dev/blog/v8-release-99)**

- Intl 개선 - Intl.Locale 객체에 새 프로퍼티 추가
    - `calendars`, `collations`, `hourCycles`, `numberingSystems`, `timeZones`, `textInfo`, `weekInfo`
- Intl Enumeration - `Intl.supportedValuesOf(code)`
    - ex) `Intl.supportedValuesOf('unit')` // ['acre', 'bit', 'byte', 'celsius', 'centimeter', ...]

### **[Electron 17 Released](https://www.electronjs.org/blog/electron-17-0)**

- 크롬 98, 노드 16.13, V8 9.8 적용
- 일렉트론 13 지원종료

### **[Prisma 3.9.0 Released: Popular Next-Gen ORM for Node.js](https://github.com/prisma/prisma/releases/tag/3.9.0)**

- 마이그레이션 이슈 해결을 돕는 CLI
    - `prisma migrate diff`, `prisma db execute`
- CockroachDB Preview 지원

# Javascript

### **[Babel 7.17.0 Released](https://babeljs.io/blog/2022/02/02/7.17.0)**

- Decorators proposal 지원
- Regexp - v flag를 붙이면 Extended set notation 등 3가지 새로운 정규식 기능

### **[VSCode 1.64](https://code.visualstudio.com/updates/v1_64)**

- Side Panel - 양쪽에 패널을 띄우는 등 레이아웃 변경 가능
- Terminal - Y응답을 할 때 엔터 자동입력
- Debugging
    - 바이너리 데이터(Hex) 보기, 수정 지원
    - JS디버깅 - BreakPoint에서 Exclude callers 제외 ex) 특정 이벤트가 호출한것만 남기고 제외하여 이벤트 핸들러를 통한 호출만 보기
- 마크다운에서 이미지 경로 인텔리전스
- 웹용 VSCode(vscode.dev) PWA 지원 - 오프라인 지원(호스트에 설치 가능)

### BRIEF

- [https://twitter.com/dan_abramov/status/1488956873390923780](https://twitter.com/dan_abramov/status/1488956873390923780)
    - [].join(', ') 대신에 Intl.ListFormat 을 사용하여 언어별 대응
- [https://twitter.com/dan_abramov/status/1488956873390923780](https://twitter.com/dan_abramov/status/1488956873390923780)
    - Dan abramov 의 sublime text4 후기
- [https://github.com/facebook/jest/pull/11529#issuecomment-1027152470](https://github.com/facebook/jest/pull/11529#issuecomment-1027152470)
    - Jest는 페이스북의 도구지만 지난 몇년간 페이스북에서 Jest에 작업하지 않음

### Release

- **[MDX 2.0](https://mdxjs.com/blog/v2/)**
- **[Partytown 0.3](https://github.com/BuilderIO/partytown)**
- **[Recoil 0.6](https://recoiljs.org/blog/2022/01/28/0.6.0-release/)**

### **[Speeding Up VS Code Extensions in 2022](https://jason-williams.co.uk/speeding-up-vscode-extensions-in-2022)**

- VSCode 아키텍처 기본
- VSCode의 익스텐션 로드를 빠르게 하기 위해 번들링하기

### **[A-Frame 1.3: A Framework for Building WebVR Experiences](https://github.com/aframevr/aframe/releases/tag/v1.3.0)**

- AFrame 1.3 릴리즈
- Vive, Rift, Quest, Browser 에서 작동하는 VR 웹 프레임워크

### **[WebVM.io](https://webvm.io/)**

- 서버리스 virtual Linux 환경 - html5/WASM 으로 클라이언트 사이드에서 실행
- [https://leaningtech.com/webvm-server-less-x86-virtual-machines-in-the-browser/](https://leaningtech.com/webvm-server-less-x86-virtual-machines-in-the-browser/)