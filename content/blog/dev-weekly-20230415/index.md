---
title: dev-weekly 2023-04-15
date: "2023-04-15T11:00:00.000Z"
description: "dev-weekly 2023-04-15"
tags: ["javascript", "css", "node"]
---

# CSS

### **[The relative font weight axis — how variable fonts ease font weight transitions](https://www.stefanjudis.com/today-i-learned/the-relative-font-weight-axis-how-variable-fonts-ease-font-weight/)**

- variant font를 사용하고 font-variation-settings 프로퍼티를 이용하여 weight 단위로 다운로드 하지 않고, 하나의 폰트만 다운로드 하여 조정하기

### **[Debug Layout Problems Using 1 Line of CSS](https://www.youtube.com/shorts/aKIanwb5FjE)**

- 한 줄의 코드로 CSS overflow로 가로스크롤 생긴 부분 찾아내기
- (FF는 브라우저가 기능 제공) 이 영상에선 `* { border: 1px solid }` 를 주고 육안으로 확인

### **[Emoji Lists, The Good Way?](https://chriscoyier.net/2023/04/07/emoji-lists-the-good-way)**

- list에 이모지를 사용하면 voice over는 이모지도 읽어주는 이슈
- voice over를 고려하여 컨텐츠가 아니라 symbol 로 추가하기

### **[New HTML Element: <search>](https://alvaromontoro.hashnode.dev/new-html-element-search)**

- HTML에 새로운 엘리먼트 search 추가
- form control이 포함되어야 함

# Node

### **[Trying Node's Built-In Test Runner](https://nodeweekly.com/link/138027/154188e1e3)**

- nodejs의 `node:test` 사용법
- 병렬 테스트 - 테스트 신택스, BDD 신택스, 테스트 레포트 등
- CI 셋팅 예제, ESM 모듈 목킹, TS파일 테스팅 등
- node v20.0에서 테스트 러너 안정화될 예정

### **[Introducing Socket AI – ChatGPT-Powered Threat Analysis](https://socket.dev/blog/introducing-socket-ai-chatgpt-powered-threat-analysis)**

- ChatGPT와 AI 기반 소스 코드 분석을 활용하여 npm, PyPI 패키지 검사
- AI 경고는 절대적인 분석이 아닌 조언. AI에 데이터를 입력하는데 한계 존재.
- AI 분석 소개 - 정보 유출, 인젝션 취약점, 자격 증명 노출, 잠재적인 취약점, 백도어 등

# Javascript

### **[Testing Localhost on Multiple Devices](https://www.silvestar.codes/articles/testing-localhost-on-multiple-devices/)**

- 맥, 윈도우에서 공유기 IP를 확인하여 접근하기
- expose 도구 사용하기 - ngrok, cloudflared(npm package)
- netlify에서 drag and drop deploy 기능 이용하기

### **[The JavaScript Equality Table Game](https://eqeq.js.org/#ko)**

- JS의 == 의 해석으로 하는 지뢰찾기 게임

### **[Ranger: JS Range Syntax for Anything](https://dev.to/jonrandy/ranger-js-range-syntax-for-anything-4djc)**

- js-ranger라는 패키지 소개. Number.prototype 을 통한 신택스 해킹
- `const numbers = 1[[...5]]` // [1,2,3,4,5]

### **[Reveal.js 4.5: An HTML Presentation Framework](https://github.com/hakimel/reveal.js/releases/tag/4.5.0)**

- 웹으로 프레젠테이션 만드는 도구 Reveal 4.5 릴리즈
    - 슬라이드 점프 기능, 테마들 추가, live reload 향상

### Release

- [Sandpack 2.6](https://github.com/codesandbox/sandpack/releases/tag/v2.6.0)
- [Partytown 0.8](https://github.com/BuilderIO/partytown/releases/tag/v0.8.0)
- [mui-x 6.1](https://github.com/mui/mui-x/releases/tag/v6.1.0)

# ETC

### **[Release Notes for Safari Technology Preview 167](https://webkit.org/blog/14100/release-notes-for-safari-technology-preview-167/)**

- &, text-transform, shape-outside 등 구현
- JS, WASM, Media, Web API 등 버그 픽스

### **[Iconhunt: A Search Engine for 150,000+ Icons](https://www.iconhunt.site/)**

- [https://iconify.design/](https://iconify.design/) 를 기반으로 아이콘을 검색기능과 노션용 링크, 피그마용 코드, 다운로드 등 제공