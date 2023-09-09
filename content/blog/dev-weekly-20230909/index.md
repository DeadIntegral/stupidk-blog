---
title: dev-weekly 2023-09-09
date: "2023-09-09T11:30:00.000Z"
description: "dev-weekly 2023-09-09"
tags: ["javascript", "node", "css"]
---
# CSS

### **[CSS Transitions Level 2](https://www.w3.org/TR/2023/WD-css-transitions-2-20230905/)**

- CSS Transition Level2 스펙 첫 번째 Public Working Draft공개

### **[Adapting to the new multi-keyword syntax of display](https://developer.mozilla.org/en-US/docs/Web/CSS/display/multi-keyword_syntax_of_display)**

- display 멀티 밸류
- `display: block flex` 는 block의 자식들은 flex로 배치
- display의 새로운 명칭들 - [https://drafts.csswg.org/css-display/#display-value-summary](https://drafts.csswg.org/css-display/#display-value-summary)

# Node

### **[Node v20.6.0 (Current)](https://nodejs.org/en/blog/release/v20.6.0)**

- `.env` 환경 변수 구성을 위한 파일 지원(built-in)
- INI 파일 포맷을 따라야 하며, 각 라인은 key=value 로 구성.

### **[Yes, there's an npm package called @(-.-)/env and some others like it](https://www.bleepingcomputer.com/news/technology/yes-theres-an-npm-package-called-env-and-some-others-like-it/)**

- `-`, `@!-!` `--hepl` 과 같은 이름의 패키지들이 존재.
- `-` 는 다운로드 수가 70만 이상. 모두가 악성은 아니지만 오타와 유사한 악성 패키지 존재할 수 있는 이슈

### **[Tracking Errors in a Node.js Application](https://blog.appsignal.com/2023/08/30/tracking-errors-in-a-nodejs-application.html)**

- 커스텀 오류 핸들러 만들기
- 프로그래밍 오류 처리하기
    
    ```jsx
    process.on("uncaughtException", (err) => {})
    process.on("unhandledRejection", (err) => {})
    ```
    

### Release

- [marked v8.0.0](https://github.com/markedjs/marked/releases/tag/v8.0.0)

# Javascript

### **[Astro 3.0](https://astro.build/blog/astro-3/)**

- View Transitions 제공
- 렌더링 성능 향상(v2.9 대비 30%)
- 이미지 최적화
    - vercel 이미지 서비스 지원
    - @squoosh/libSharp 는 sharp로 마이그레이션
    - 리모트 이미지 최적화 지원
- SSR 향상 - vercel과 공식 호스팅 파트너십 체결
- HMR 향상 - React fast refresh 지원
- 빌드 아웃풋 최적화 - 클래스는 data-*로 대체. 아웃풋 축소 등

### **[Browser Video Players Review](https://adrianroselli.com/2023/09/browser-video-players-review.html)**

- 각 OS, 브라우저별 Video 태그 사용시 노출되는 플레이어들 테스트
- 키보드 접근, 스크린 리더 등 다양한 항목들 비교 분석 (MDN과는 다른 느낌의 호환성)

### **[How to Create a Chrome Extension in 10 Minutes Flat](https://www.sitepoint.com/create-chrome-extension-10-minutes-flat/)**

- 크롬 확장 프로그램 만들기 기초 설명

# ETC

### **[With version 117, Firefox finally speaks Chrome's translation language](https://www.theregister.com/2023/08/31/firefox_117/)**

- 파이어폭스 117부터 `about:config` 에서 `browser.translations.enable` 를 설정하면 주소창에 번역 아이콘 추가

### **[Towards HTTPS by default](https://blog.chromium.org/2023/08/towards-https-by-default.html)**

- 지난 몇년동안 사용자 탐색의 90% 이상이 https로 전환
- 크롬은 HSTS처럼 http가 명시적인 링크에도 https로 업그레이드해서 작동할 것
    - 업그레이드가 실패할 경우(잘못된 인증서 혹은 404) http로 제공

### **[Where to Put Focus When Deleting a Thing](https://adrianroselli.com/2023/08/where-to-put-focus-when-deleting-a-thing.html)**

- 그룹에서 항목 삭제 시 포커스 처리하기
    - 리스트에서 아이템을 삭제할 때는 이전에 해당하는 컨트롤로 포커싱하기
    - 만약 첫 번째 아이템을 삭제하면 컨테이너로 포커스 이동하기