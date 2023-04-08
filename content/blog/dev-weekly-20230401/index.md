---
title: dev-weekly 2023-04-01
date: "2023-04-01T014:40:00.000Z"
description: "dev-weekly 2023-04-01"
tags: ["javascript", "css", "node", "web", "typescript", "deno"]
---

# CSS

### **[Why APCA as a New Contrast Method?](https://git.apcacontrast.com/documentation/WhyAPCA.html)**

- WCAG 의 색상 대비는 수리적인 부분인데 가독성 면에서의 대비는 인식과 뇌의 시각적 차이.
- 새로운 방법이자 교체 후보인 APCA(Accessible Perceptual Contrast Algorithm) 소개

### **[CSS Nesting](https://developer.chrome.com/articles/css-nesting)**

- 크롬 112, 사파리 16.2에서부터 CSS Nesting 적용
- 신택스에 대한 소개
    
    ```css
    .card {
      .featured & & & {} /* .featured .card .card .card */
    }
    ```
    
- nesting parser에 대한 설명

### **[CSS Flux Capacitor](https://codepen.io/konstantindenerz/pen/yLxpjYz)**

- HTML, CSS만으로 만든 일러스트레이터. @property 활용.

### **[Detecting noscript with MediaQuery in Firefox](https://www.w3.org/TR/mediaqueries-5/#descdef-media-scripting)**

- 파이어폭스에서 `@media (scripting: none)` 지원

# Node

### **[Are Half of New npm Packages Just Junk?](https://blog.sandworm.dev/one-in-two-new-npm-packages-is-seo-spam-right-now)**

- npm 에 제출되는 새로운 패키지 중 절반 이상이 SEO 스팸.
- README 단일 파일만 존재. 러시아 텔레그램, 책과 비디오 광고, 포트나이트 피싱 등
- sandworm(글 작성 회사)의 대응

### **[The Landscape of npm Packages for CLI Apps](https://blog.kilpatrick.cloud/posts/node-cli-app-packages/)**

- CLI 앱용 패키지는 대부분 2015년 이전에 만들어졌고, TS로 다시 작성한것 패키지는 없음
- Argument Parsing, Output Styling, User Input 의 세 카테고리에서 인기있는 도구들을 비교 및 설명
- 프레임워크 소개 - oclif, ink, vorpal

### **[Nano JSX: A Lightweight SSR-First JSX Library](https://nanojsx.io/)**

- VDom을 사용하지 않는 JSX 라이브러리

### **Release**

**[sharp 0.32.0](https://github.com/lovell/sharp/releases/tag/v0.32.0)**

**[strapi 4.9.0](https://github.com/strapi/strapi/releases/tag/v4.9.0)**

**[prisma 4.12.0](https://github.com/prisma/prisma/releases/tag/4.12.0)**

# Javascript

### **[WebKit Features in Safari 16.4](https://webkit.org/blog/13966/webkit-features-in-safari-16-4/)**

- badging API - iOS에서 배지 수 표시 가능
- 웹 컴포넌트, media query level4
- font-size-adjust
- `@property` at-rule 지원
- offscreenCanvas, fullscreen API, Screen Wake Lock API, User Activation API
- macOS Monterey, macOS Big Sur 에서도 AVIF 지원

### **[Day 100: it's over, or is it!?](https://www.matuzo.at/blog/2023/100daysof-day100/)**

- 모던 CSS 100일 종료. 지난 138일 (업무시간 100일) 동안의 공부 공유 후기
- [https://www.matuzo.at/blog/2022/100-days-of-more-or-less-modern-css/](https://www.matuzo.at/blog/2022/100-days-of-more-or-less-modern-css/)

### **[JavaScript import maps are now supported cross-browser](https://web.dev/import-maps-in-all-modern-browsers/)**

- import map에 대한 소개. 이 글에서는 3개 엔진이지만 사파리 16.4에서도 지원하여 메이저4개 브라우저 모두가 지원

### **[React Labs: What We've Been Working On](https://react.dev/blog/2023/03/22/react-labs-what-we-have-been-working-on-march-2023)**

- 리액트 팀의 작업 공유
- React Server Component, Asset Loading, Document Metadata, Offscreen Rendering
- 리액트 컴파일러 React Forget. 리액트의 멘탈 모델 대로라면 너무 많이 렌더링 될 수 있고, React forget의 목표는 적절한 양의 반응을 하는 것.
    - 구현 관점에서는 automatically memoizing이지만, 컴파일러 이해 측면에선 reactivity framing 이 더 좋음

### **[Microsoft rebuilt Teams from the ground up, promises 2x faster performance](https://techcrunch.com/2023/03/27/microsoft-rebuilds-teams-promises-2x-faster-performance/)**

- MS 팀즈 AngularJS에서 리액트로 전환. 일렉트론에서 MS Edge Webview2 렌더링 엔진으로 변경

### **[Announcing Rome v12](https://rome.tools/blog/2023/03/28/rome12/)**

- JSON 파일 지원 (로마가 진단)
- TS 4.7, 5.0 지원, 린트 옵션 추가

### **[Solid **v1.7.0 - U Can't Type This**](https://github.com/solidjs/solid/releases/tag/v1.7.0)**

- v2.0의 마이그레이션 시작 버전.
- TS지원 향상, 모든 자식의 에러 검출 가능한 catchError, dev tools 안정화

### **[Visual Studio Code March 2023](https://code.visualstudio.com/updates/v1_77)**

- TS 5.0.2 지원
- switch case에서 … 을 사용하면 인자의 타입을 파싱하여 case 문 스캐폴딩
- 파이썬 환경 개선
    - python runtime이 없어도 conda 환경 나열
    - 노트북 저장 시 포맷 활성화, 활성화된 노트북 찾기, 노트북 내에서 스크롤 가능한 출력 영역
    - 노트북 출력에 대해 검색 지원

### **Release**

**[Ionic 7.0](https://ionic.io/blog/ionic-7-is-here)**

**[ink v.4.1.0](https://github.com/vadimdemedes/ink/releases/tag/v4.1.0)**

**[SVGR v7.0.0](https://github.com/gregberge/svgr/releases/tag/v7.0.0)**

**[Qwik 0.100](https://github.com/BuilderIO/qwik/releases/tag/v0.100.0)**

- 0.25 다음버전으로 0.100 업데이트. 모든 브레이킹 체인지를 완료했고 여기서 1.0 릴리즈는 Vite, TS, Node 외에는 변경없음

# ETC

### **[MySQL Boolean 컬럼](https://medium.com/daangn/mysql-boolean-%EC%BB%AC%EB%9F%BC-7abd9b35c664)**

- mysql boolean 구현과 작동 방식 (컬럼 타입으로는 있지만 boolean이 아닌 MySQL의 특성)

### **[An in-depth course on images for the web.](https://web.dev/learn/images/)**

- 초보자, 고급자 모두를 위한 이미지 문서 정리
- 효율적인 요청부터 렌더링까지 이미지가 작동하는 방식에 대한 전체적인 정리