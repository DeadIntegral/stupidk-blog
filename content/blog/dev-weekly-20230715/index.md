---
title: dev-weekly 2023-07-15
date: "2023-07-15T15:15:00.000Z"
description: "dev-weekly 2023-07-15"
tags: ["javascript", "css", "node"]
---
# CSS

### **[New Viewport Units](https://ishadeed.com/article/new-viewport-units/)**

- 브라우저 구현마다 다른 vh
    - 검색창을 포함하는 브라우저와 그렇지 않은 브라우저
- 검색창을 포함하지 않는 svh, 포함하는 lvh, 동적 뷰포트 dvh에 대한 설명과 이를 사용한 문제 해결

### **[What’s your type? Try these tests to pick the perfect font for you.](https://www.washingtonpost.com/technology/interactive/2023/best-font-you-test-types-styles)**

- 폰트에 따른 영향과 실험. (페이지 내에서 테스트)
- 모두를 만족하는 폰트는 없음.
- 폰트의 비율, 대비, 간격, 높이가 어떠한 영향을 미치는지 간략한 설명 제공

# Node

### **[Node v20.4.0 (Current)](https://nodejs.org/en/blog/release/v20.4.0)**

- setTimeout, setInterval와 같은 테스트를 위한 `MockTimers`제공

### **[ECMAScript Modules in Node.js](https://www.typescriptlang.org/docs/handbook/esm-node.html)**

- TS에서 ESM을 사용하는 공식 가이드문서.

# Javascript

### **[driver.js](https://driverjs.com/)**

- 도움말 플로우를 작성 가능한 의존성 없는 라이브러리 [driverjs 1.0.3 release](https://github.com/kamranahmedse/driver.js/releases/tag/1.0.3)
- TS로 재작성.

### **[Component party](https://component-party.dev/)**

- UI 라이브러리 코드 스니펫을 비교해서 보여주는 사이트.
- 스니펫, 라이브러리들을 선택하면 해당 스니펫에 대한 다양한 구현체 샘플 비교 보기 제공
- 상태관리, 템플레이팅, 라이프사이클, 컴포넌트 컴포지션, 폼 인풋 등 다양한 스니펫 제공
- Svelte, React, Vue3, Solid, Qwik, Angular, Lit, Ember 등 제공

### **[Prisma 5: Faster by Default](https://www.prisma.io/blog/prisma-5-f66prwkjx72s)**

- Prisma 5.0 릴리즈. 서버리스 환겨에서 시작 성능 개선.
- GraphQL과 유사한 프로토콜에서 JSON 기반 프로토콜로 변경 (CPU, 메모리 오버헤드 개선)
- 의존성 감소, 쿼리 엔진 내부 최적화, 스키마 변환 병렬로 진행

### **[P5.js 1.7](https://github.com/processing/p5.js/releases/tag/v1.7.0)**

- WebGL 2 지원, 더 부드러운 카메라 이동을 위한 도구 지원
- 프레임 버퍼 개선

### **[Ember 5.1 Released](https://blog.emberjs.com/ember-released-5-1/)**

- Ember 5.1 릴리즈. 안정적인 TS 지원 (엠버에서 빌드된 타입 게시)
- tsconfig target ES2021로 변경

### **[Optional Chaining Assignment](https://github.com/nicolo-ribaudo/proposal-optional-chaining-assignment)**

- `expr1?.[key] = val` 옵셔널 체이닝 할당 제안. (스테이지1)

### **[Electron-vite](https://electron-vite.org/)**

- 기존의 vite 기반 일렉트론 템플릿들이 갖고있는 문제를 해결하려고 만든 도구
    - 소스 코드 보호, 추론, 프론트엔드 프레임워크 선택, 구성 난이도 등
- 번들러는 NodeJS 와 브라우저 환경 모두 처리해야 하는데 Vite는 이에 적합.

### **Release**

- [octokit.js 3.0](https://github.com/octokit/octokit.js/releases/tag/v3.0.0)
- [preact 10.16.0](https://github.com/preactjs/preact/releases/tag/10.16.0)

# ETC

### **[Prettier 3.0: Hello, ECMAScript Modules!](https://prettier.io/blog/2023/07/05/3.0.0.html)**

- Prettier 3.0 릴리즈.
- ESM 으로 마이그레이션. CommonJS 지원.
- 다크다운 형식 변경(라틴문자, 중국어, 일본어 사이의 공백 삽입 제거), 한국 단어 내의 줄바꿈 금지
- trailing comma 기본값 all로 변경, pure css 파서 추가
- node 10, 12 지원 중단

### **[The case against self-closing tags in HTML](https://jakearchibald.com/2023/against-self-closing-tags-in-html/)**

- `/>` 은 2000년에 HTML 파서와 XML 파서 모두 호환하게 작성하는것이 권장이라 지원.
- 2008년 HTML5 가 등장하면서 XHTML에 도입된 XML 요구 사항 제거

### **[State Of Npm 2023: The Overview](https://blog.sandworm.dev/state-of-npm-2023-the-overview)**

- NPM의 현 상태
- 전체 패키지 330만개, 총 버전 수 3400만개, 지난 1년 생성된 패키지 139만개(그 중 56만개 스팸)
- 전체 패키지 크기 24.17TB, 평균 패키지 크기 416KB
- 키워드 1위 react 97k, 2위 typescript 43k, javascript 36k, vue 35k

### **[Introducing passwordless authentication on GitHub.com](https://github.blog/2023-07-12-introducing-passwordless-authentication-on-github-com/)**

- Github PassKey 베타 시작.
- 깃헙에서 패스키 설정하는 가이드 및 패스키가 암호를 대체하는 방법 설명.

### **[WCAG 2.2, quick and simplified](https://medium.com/design-ibm/wcag-2-2-quick-and-simplified-73c3ff66b065)**

- 접근성 지침 새 버전 7월 초에 W3C 제안 권장사항이 될 것.
- 새로운 9가지 요구사항. 포커스, 드래그, 크기, 도움말, 중복항목, 인증 관련.

### **[terminalizer](https://github.com/faressoft/terminalizer)**

- 터미널을 기록하고 gif를 생성하는 도구.
- [https://asciinema.org/](https://asciinema.org/) 와 유사

### **[tinypool](https://github.com/tinylibs/tinypool)**

- 38kb의 의존성 없는 worker thread pool 구현.
- logical core 대신 physical core 사용