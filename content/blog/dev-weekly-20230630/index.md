---
title: dev-weekly 2023-06-30
date: "2023-06-30T12:40:00.000Z"
description: "dev-weekly 2023-06-30"
tags: ["javascript", "css", "node", "etc"]
---
# CSS

### **[CSS Drawings A Single Div CSS Art Project by Alvaro Montoro](https://cssdrawings.com/)**

- 하나의 div(article)에 after, before를 사용해 만든 CSS Art 들

# Node

### **[NestJS v10 is now available!](https://trilon.io/blog/nestjs-10-is-now-available)**

- NestJS10 소개. SWC 제공 (-b swc 플래그 혹은 compilerOptions.builder 셋팅으로 사용 가능)
- 테스트에서 모듈 오버라이딩, Redis에서 와일드카드 구독
- Node v12 지원 중단, cli 플러그인은 TS 4.8 이상 지원.

### **[Nightwatch.js 3.0: End-to-End Web Testing Framework](https://nightwatchjs.org/)**

- browserstack의 E2E 테스팅 제품 Nightwatch 3.0 릴리즈.
- Browser, Native Mobile 등 지원 (xcode, andriod sdk 16+ 필요)
- [https://github.com/nightwatchjs/nightwatch](https://github.com/nightwatchjs/nightwatch)

### **[node-google-spreadsheet 4.0 Release](https://github.com/theoephraim/node-google-spreadsheet/releases/tag/v4.0.0)**

- TS 재작성. google auth library 의존성 수정. 문서 삭제 지원 등.
- 애플리케이션 디폴트 자격 증명 지원(일부 환경에서는 자동 주입)

### **[The massive bug at the heart of the npm ecosystem](https://blog.vlt.sh/blog/the-massive-hole-in-the-npm-ecosystem)**

- NPM 생태계에서 package.json과 manifest가 달라도 되는 버그.
- manifest에 없는 패키지를 설치시킬 수 있음.
- NPM 와 써드파티인 Snyk, CNPM, Cloureflare Mirror, Skypack, UNPKG, JSPM, Yarn 등에 영향

# Javascript

### **[TypeScript 5.2's New Keyword: 'using'](https://www.totaltypescript.com/typescript-5-2-new-keyword-using)**

- `Symbol.dispose` 소개
- 비동기 처리가 끝나면 자동으로 dispose시키게 해주는 using, dispose 패턴 예제 설명

### **[Announcing Stencil v4.0.0](https://ionic.io/blog/announcing-stencil-v4-0-0)**

- IE, 크롬 엣지 이전 버전, 사파리10 지원 종료
- Node14 지원종료.
- [https://github.com/ionic-team/stencil/blob/v4.0.0/BREAKING_CHANGES.md#stencil-v400](https://github.com/ionic-team/stencil/blob/v4.0.0/BREAKING_CHANGES.md#stencil-v400)

### **[WebPerf Snippets](https://webperf-snippets.nucliweb.net/)**

- 웹 브라우저 콘솔이나 snippet에서 복붙해서 사용할 퍼포먼스 스니펫 모음
- Core Web Vital, 인터랙션, 로딩 관련한 스니펫들.

### **[Ecma International approves new standards](https://www.ecma-international.org/news/ecma-international-approves-new-standards-at-the-125th-general-assembly-27-june-2023/)**

- 2023년 6월 27일 제네바에서 개최된 125회 총회에서 다음 문서들 승인
    - ECMA-262 14판 - 언어 스펙
    - ECMA-402 10판 - 국제화 API 스펙
    - ECMA-419 2판 - 임베디드 시스템 API 스펙
    - ECMA-423 1판 - 홀로그램 데이터 저장 디스크(HDSD) - 디스크당 1TB

### **[Why doesn't TypeScript properly type Object.keys?](https://alexharri.com/blog/typescript-structural-typing)**

- Object.keys를 사용하면 추론못하는 TS
- `keys<T extends object>(o: T): (keyof T)[];` 정도로 기입해도 되는데 못하는 이유는 structural type system 때문
- 예제로 살펴보면 구조적 타입 시스템(타입이 포함관계일 때 런타임의 에러를 막기 위해서)

### **Release**

- [Ember 5.0 Released](https://blog.emberjs.com/ember-5-0-released/)
- [styled-components v6.0.0](https://www.notion.so/2023-06-30-32c2bea9e6e9481da8665edcf02492be?pvs=21)
- [remix v1.18.0](https://github.com/remix-run/remix/releases/tag/remix%401.18.0)
- [radash v11.0.0](https://github.com/rayepps/radash/releases/tag/v11.0.0)

# ETC

### **[GN+](https://news.hada.io/plus)**

- AI가 요약한 최신 뉴스를 긱뉴스에서 제공하는 서비스

### **[Introducing the MDN Playground: Bring your code to life!](https://developer.mozilla.org/en-US/blog/introducing-the-mdn-playground/)**

- MDN에 playground 추가. 기존 라이브 샘플과의 통합을 위해 다른 playground를 사용하지 않고 구축.
- OpenAI를 사용하여 코드를 설명해주는 기능 제공.
- monaco를 고려했지만 보다 가벼운 codemirror 를 사용하여 구축.

### **[[css-properties-values-api] Enable on nightly.](https://phabricator.services.mozilla.com/D182111)**

- Firefox Nightly 에서 @propety at rule 지원

### **[5 reasons why a browser and mail combination is worth it.](https://vivaldi.com/blog/how-to/5-reasons-why-a-browser-and-mail-combination-is-worth-it/)**

- 비발디 브라우저에 mail 클라이언트 내장.

### **[Useful DevTools Tips and Tricks](https://www.smashingmagazine.com/2023/06/popular-devtools-tips/)**

- 개발자도구 팁, 트릭 모음 15가지
    - 파이어폭스에서 개발자도구 셋팅(F1) 변경하여 부분 측정 - 거리와 면적
    - 크롬기반 브라우저에서 Coverage 를 사용하여 미사용코드 감지
    - 페이지의 모든 이미지 다운로드
    - 엣지에서 3D 보기 - 크롬 기반 브라우저의 Layer와 유사