---
title: dev-weekly 2023-05-27
date: "2023-05-27T12:00:00.000Z"
description: "dev-weekly 2023-05-27"
tags: ["javascript", "css", "node"]
---

# CSS

### **[Dark Mode in 3 Lines of CSS and Other Adventures](https://dev.to/madsstoumann/dark-mode-in-3-lines-of-css-and-other-adventures-1ljj)**

- System color를 이용해 3줄로 다크 모드 만들기
- only css로 color-scheme 토글 만들기 등 다크모드 환경 구축하는 예제

# Node

### **[State of Node.js Performance 2023](https://blog.rafaelgss.dev/state-of-nodejs-performance-2023)**

- Nodejs 16, 18, 20 의 재현 가능한 성능 비교.
- 성능 회귀 발생하는 케이스, autocannon과 같은 도구를 사용했을 때 다른 지표가 나오는 케이스 등 다양한 케이스에서의 지표.

# Javascript

### **[Introducing the popover API](https://developer.chrome.com/blog/introducing-popover-api/)**

- 크롬 114부터 제공. dialog와는 다르게 자체적인 시멘틱을 제공하지 않음.

### **[11 HTML best practices for login & sign-up forms](https://evilmartians.com/chronicles/html-best-practices-for-login-and-signup-forms)**

- 로그인, 회원가입 폼을 만드는 베스트 프랙티스
- autocomplete, type, button(a), focus state, 스크린 리더 …
- 두번 클릭 방지, 네트워크 레이턴시와 서버 에러 처리

### **[DeviceScript TypeScript for Tiny IoT Devices](https://microsoft.github.io/devicescript/)**

- 마이크로 컨트롤러 기반 디바이스에 TS경험을 제공하려는 MS의 노력
- 커스텀 VM 바이트코드로 컴파일
- npm, yarn, pnpm 을 통해 패키지 배포 및 사용

### **[Announcing TypeScript 5.1 RC](https://devblogs.microsoft.com/typescript/announcing-typescript-5-1-rc/)**

- 함수 선언을 다른 파일로 이동(현재 프리뷰)
- JSX에서 태그의 시작 부분을 변경하면 끝 부분도 같이 변경
- JS, TS파일에서 `@param` 작성 시 스니펫 제공
- 최적화 작업들
- 브레이킹 체인지 - 최소지원버전 ES2020, Nodejs 14.17

### **[javy: JS to WebAssembly toolchain](https://github.com/bytecodealliance/javy)**

- JS to WASM 툴체인 도구 javy 1.0 릴리즈. (작성 시점 1.0.1)

# ETC

### **[WebKit Features in Safari 16.5](https://webkit.org/blog/14154/webkit-features-in-safari-16-5/)**

- nesting css, 웹상에서 애플페이 지원

### **[The Rhythm of Your Screen](https://www.chrbutler.com/the-rhythm-of-your-screen)**

- 좋은 인터랙션에 관한 글.
- 좋은 인터랙션 디자인은 주의력 관리에 관한 것. 문제는 “스크롤 할 것인가”가 아니라 보이는 정보를 처리할 수 있을 만큼 천천히 스크롤 할 것인가.
- 좋은 디자인에 대한 팁 소개

### **[Deno 1.34: deno compile supports npm packages](https://deno.com/blog/v1.34)**

- npm 패키지로 컴파일하는 deno compile 지원. (싱글 바이너리 파일)
- IP 주소를 포함한 TLS 인증
- API 변경. Deno.serve()는 상위 호환성을 위해 안정화 연기

### **[Be Careful Using ‘Menu’](https://adrianroselli.com/2023/05/be-careful-using-menu.html)**

- menu 라는 단어 사용에 대한 주의. 컨트롤에 맞는 용어와 그에 대한 설명.
- menu, menuitem 요소는 구현안되고 중단.

### Release

- **[Astro 2.5](https://astro.build/blog/astro-250/)**
- **[Preact 10.15.0](https://github.com/preactjs/preact/releases/tag/10.15.0)**
- **[MapLibre GL JS v3](https://maplibre.org/news/2023-05-23-maplibre-gl-js-v3/)**