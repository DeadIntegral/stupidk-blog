---
title: dev-weekly 2023-02-25
date: "2023-02-25T14:00:00.000Z"
description: "dev-weekly 2023-02-25"
tags: ["javascript", "css", "node"]
---

# CSS

### **[Improved Font Fallbacks](https://developer.chrome.com/blog/font-fallbacks)**

- `size-adjust`, `ascent-override`, `descent-override`, `line-gap-override` API를 대한 설명
- acscent, desent line gap을 조정하여 fallback 폰트의 글리프를 조정하는 방법
- size-adjust를 통해 fallback 폰트의 글리프를 조정하는 방법
- OS별 폰트 계산법 및 폰트 테이블에 대한 설명

### **`[(255,255,255)` is the Highest Specificity](https://www.bram.us/2023/02/21/255255255-is-the-highest-specificity)**

- 블링크 소스로 살펴보는 CSS Specificity 한계치
- 크롬, 사파리는 255, FF는 1023. (A, B, C) 포맷으로 계산하지만 overflow가 나면 자체적으로 clamp (ex: 1, 257, 0 ⇒ 1, 255, 0)

### **[A Step-By-Step Guide To Building Accessible Carousels](https://www.smashingmagazine.com/2023/02/guide-building-accessible-carousels)**

- 정말 캐러셀이 필요한지 확인하기 - 89%의 유저는 첫 번째 슬라이드만 사용
- 접근성 있는 캐러셀 만들기 - 일시중지, 중지 버튼 만들기, 포커스 온 되면 영구 정지하기 등
- 색상대비, 포인터 입력, 스크린 리더기의 식별을 위한 속성들, 포커스 순서 등

### **[HTML Input Types](https://markodenic.com/html-input-types)**

- input type 별 간단한 설명 - month, search, url, week

# Node

### **[Node v19.7.0 (Current) Released](https://nodejs.org/en/blog/release/v19.7.0/)**

- Ada WHATWG 호환 URL parser (최대 87% 성능 향상)
- Single executable applications 실험적 지원 (아직 80MB)

### **[Announcing Sandpack 2.0 and a Node.js runtime for any browser](https://codesandbox.io/blog/announcing-sandpack-2)**

- 브라우저에서 서버 측 코드를 실행할 수 있는 도구 Nodebox를 도입한 Sandpack 2.0 릴리즈
- napi 혹은 그에 준하는 로울 레벨 패키지는 실행 불가. WASM, JS 모듈만 실행 가능. raw 소켓이 지원되지 않아 아직 브라우저에서 Postgres, MongoDB, MySQL은 사용 불가
- 웹 컨테이너는 SharedArrayBuffer등을 사용해서 Safari에서 사용 할 수 없고 Cross Origin Ioslation 헤더 작업 필요.

### ****[The State of Node.js Core ft. Colin Ihrig | JS Drops](https://www.youtube.com/watch?v=OIrGEgMwPvc)****

- NodeJS 코어 팀의 Nodejs 코어 현황 프레젠테이션 (유튜브)

### Release

- **[LDAPjs 3.0](https://github.com/ldapjs/node-ldapjs/releases/tag/v3.0.0)**
- ****[Storybook 7 Docs](https://www.notion.so/2023-02-25-f2b73474e066406a95aad25255bcd5f0)****
- **[Angular 15.2](https://github.com/angular/angular/releases/tag/15.2.0)**
- **[React Testing Library 14.0](https://github.com/testing-library/react-testing-library/releases/tag/v14.0.0)**

# Javascript

### **[The ECMAScript 2023 Language Specification](https://tc39.es/ecma262/)**

- ECMA 읽는법 - [https://timothygu.me/es-howto](https://timothygu.me/es-howto/)

### **[Let's Build a Chrome Extension That Steals Everything](https://mattfrisbie.substack.com/p/spy-chrome-extension)**

- 크롬 확장을 통해 할 수 있는 최대한의 것.
    - background Service Worker, Popup Page, Content Script의 특징들
    - 백그라운드 페이지의 네트워크 트래픽은 ad block, privacy extension의 영향을 받지 않음
- 얼마나 다양한 정보를 훔칠 수 있는지 위협요소 나열

### ****[Next.js 13.2](https://nextjs.org/blog/next-13-2)****

- 새로운 Metadata API 제공 - 서버 컴포넌트인 모든 레이아웃, 페이지에 메타데이터 셋팅 가능
- 서버 컴포넌트를 위한 MDX, Rust MDX 파서
- next/link 사용 시 앱을 탐색하여 존재하지 않는 경로 입력 시 TS 에러
- 오류 오버레이 개선, 터보팩 개선, 캐시 개선

### **[Mermaid 10.0](https://github.com/mermaid-js/mermaid/releases/tag/v10.0.0)**

- ESM Only. CJS 지원 중단.
- `<script src="https://cdn.jsdelivr.net/npm/mermaid@9/dist/mermaid.js"></script>` 를 통해 9 이용 가능