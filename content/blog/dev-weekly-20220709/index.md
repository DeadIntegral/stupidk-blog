---
title: dev-weekly 2022-07-09
date: "2022-07-09T15:15:00.000Z"
description: "dev-weekly 2022-07-09"
tags: ["javascript", "css", "node"]
---
# CSS

### **[The Joy of Variable Fonts: Getting Started on the Frontend](https://evilmartians.com/chronicles/the-joy-of-variable-fonts-getting-started-on-the-frontend)**

- variable font 사용방법
    - `tech('variations')` 를 사용해 브라우저에게 노티하기
- font-variation-settings 사용법 및 주의사항(글 작성 시점에 지원되는 브라우저는 FF뿐)

### **[Single Element Loaders: Going 3D!](https://css-tricks.com/single-element-loaders-going-3d)**

- 하나의 요소(엘리먼트)로 로딩 인디케이터 만들기 3D버전

### **[Are You Sure That’s a Number Input?](https://kilianvalkhof.com/2022/css-html/are-you-sure-thats-a-number-input)**

- input number를 써야 할 때와 그렇지 않을 때
- 카드번호, 우편번호 등은 잘못된 사용 예. 숫자로 구성된 것이 아니라 숫자에 써야 함
- 모바일에서 사용자에게 키보드 지원을 하기 위하서라면 `<input inputmode="numeric" />` 를 사용하기

### **[Animated House from "Up"](https://codepen.io/jh3y/pen/jOzNQyG)**

- HTML, CSS 로만 제작한 움직이는 집

# Node

### **[Bun: An Interesting New JavaScript Runtime](https://bun.sh/)**

- Node, Deno랑 다르게 Webkit/JavascriptCore 를 사용한 JS 런타임
- .env파일을 자동으로 로드 등 특징들 소개
- Zig로 작성

### **[Ways to Estimate npm Package Market Share](https://blog.isquaredsoftware.com/2022/07/npm-package-market-share-estimates/)**

- npm 패키지 마켓을 추정하는 방법
- npm 다운로드 수 비교와 CI, 호스팅 캐싱 서버, cnpm(china npm), bot 등으로 인한 영향
- npm depency 확인 및 주의사항 등

### **[yoctocolors 1.0: The Smallest and Fastest Command-Line Coloring Package](https://github.com/sindresorhus/yoctocolors)**

- 가장 작고 빠른 커맨드라인 컬러링 패키지
- chalk와 같은 라이브러리

# Javascript

### **[bundlejs: Online npm Package Bundler and Size Checker](https://bundlejs.com/)**

- 라이브러리들을 빌드하고 번들 사이즈 및 gzip 사이즈를 알려주는 서비스
- [https://bundlephobia.com/](https://bundlephobia.com/) 와 유사

### **[VSCode **version 1.69**](https://code.visualstudio.com/updates/v1_69)**

- 3way merge editor
- setting editor에서 수정된 항목 표시
- 미니맵 크기, 배율, 슬라이더 등 조절
- 터미널 - 쉘 통합, 최근 디렉토리 이동 등
- VSCode Server - WSL, Linux등에 설치 후 다른 장비에서 vscode.dev에서 연결하여 작업 가능
- 그 외 다양한 메이저 업데이트들

### **[Notion SDK for JS 2.0](https://github.com/makenotion/notion-sdk-js/releases/tag/v2.0.0)**

- 오피셜 노션 sdk 2.0 릴리즈
- [https://developers.notion.com/changelog/releasing-notion-version-2022-06-28](https://developers.notion.com/changelog/releasing-notion-version-2022-06-28)

### **[ProtoScript: Protocol Buffers Runtime and Code Generation Tool](https://github.com/tatethurston/protoscript)**

- TS로 작성된 protocol buffers 런타임 및 코드 생성 도구
- google-protobuf와 거의동일하지만 훨씬 작고, ESM 지원
- protoc의 JSON (역)직렬 변환기 생성 idiomatic JS 코드를 대체

### **[Deprank: Use PageRank to Find the Important Files in Your Codebase](https://github.com/codemix/deprank)**

- PageRnk 알고리즘을 이용해서 코드 베이스에서 가장 중요한 파일을 찾는 도구
- 소스 파일의 종속성 그래프를 작성하고, 중요도(의존성)에 따라 순위 지정