---
title: dev-weekly 2023-07-22
date: "2023-07-22T09:00:00.000Z"
description: "dev-weekly 2023-07-22"
tags: ["javascript", "css", "node"]
---
# CSS

### **[Animated SVG Logo](https://antfu.me/posts/animated-svg-logo)**

- SVG로 스트로크 애니메이션 만들기
- 피그마 펜 툴로 로고를 그리고, export한 SVG에 css 작업
    - keyframe에 stroke-dasharray 프로퍼티 사용

# Node

### **[Pacquet](https://github.com/anonrig/pacquet)**

- Rust로 만든 nodejs 패키지 매니저. 학습용도로 만든 패키지.

### **[nve 16.1.0](https://github.com/ehmicky/nve/releases/tag/16.1.0)**

- 이제 .nvmrc, package.json 등의 파일에 파일 경로로 Nodejs 버전 지칭 가능
    - `$ nve /path/to/.nvmrc npm test`
- 여러 Nodejs 버전을 실행할 때 확인된 전체 버전 출력. nve 10, 12 ⇒ nodejs 10.24.1, nodejs 12.22.12

### **[Fresh 1.3 – Simplified Route Components and More](https://deno.com/blog/fresh-1.3)**

- Deno Fresh 1.3 릴리즈
- 핸들러와 컴포넌트를 하나의 함수로 지원. (기존에 데이터를 전달하기 위한 인터페이스 문법도 하위호환 유지)
- Error Boundary, 하나의 파일에서 여러 island 내보내기 지원, Deno.serve 지원

### **[brotli-wasm](https://github.com/httptoolkit/brotli-wasm)**

- WASM을 통해 nodejs, browser를 지원하는 Brotli 인코더, 디코더

### **Release**

- [fastify 4.20.0](https://github.com/fastify/fastify/releases/tag/v4.20.0)
- [hyper-express 6.8.0](https://github.com/kartikk221/hyper-express/releases/tag/6.8.0)
- [nest 10.1.0](https://github.com/nestjs/nest/releases/tag/v10.1.0)
- [mercurius 13.1.0](https://github.com/mercurius-js/mercurius/releases/tag/v13.1.0)

# Javascript

### **[pkg-size](https://pkg-size.dev/)**

- npm 패키지의 실제 크기를 찾는 도구. 깃헙은 리포트 용도. 비공개 소스 코드
- WebContainer를 기반으로 구축되어 직접 npm을 실행하고 패키지를 설치. esbuild WASM을 사용하여 패키지 번들링
- 사이트는 정적이고 vercel에서 호스팅

### **[Storybook 7.1](https://storybook.js.org/blog/storybook-7-1/)**

- 신규 사용자를 위한 온보딩 플로우 제공.
- Tailwind, Material UI, Emotion, styled-component 에 대한 Zero Config 스타일링 지원
- 탭에 문서를 표시하지 않고, 사이드바 메뉴 항목으로 대체
- 피그마 파트너십 - Dev Mode의 파트너가 됐고 피그마를 스토리북으로 가져오기 제공

### **[How React 18 Improves Application Performance](https://vercel.com/blog/how-react-18-improves-application-performance)**

- 리액트 18 에서의 성능 향상을 읽기 좋게 풀어낸 글.
- 50ms 이상 걸리는 작업은 long task. 이는 60fps를 기반으로 하며 web.dev의 rail 문서에 보다 자세히 설명되어 있음
- 최적의 성능을 위해 long task를 최소화 해야 하고, React update는 TBT와 INP에 최적화
- 기존의 리액트 렌더링은 동기식 렌더링으로, VDOM을 그리고 이를 실제 DOM에 적용하는데 이는 단일 작업. 그동안 메인 스레드는 차단.
- 리액트 18은 concurrent renderer 도입
    - 이 렌더러는 특정 렌더링을 긴급하지 않은 것으로 표시하는 방법 제공
    - 이 경우 5ms마다 메인 스레드에 양보 (useTransition사용)
    - 컴포넌트 트리의 렌더링을 일시 중지했다가 다시 시작 가능. (기존 렌더러는 전부 아니면 전무)
- Server Component 직렬화된 컴포넌트 트리 전송 가능. html 파일이나 js 번들 없이 리액트 컴포넌트 트리 재구성
- Suspense 기존에도 있었지만 18에서는 데이터 페칭까지 확장
- cache함수 제공. 동일한 렌더 패스 내에서 동일한 인자로 함수를 호출하면 함수를 실행하지 않고 메모된 값을 사용.

# ETC

### **[Using emoji on the web](https://fullystacked.net/posts/using-emoji-on-the-web/)**

- 브라우저마다 사용하는 이모티콘 폰트가 다름
    - Apple Color Emoji, MS Segoe Color Emoji, 파이어폭스: 트위터의 Twemoji Font
- 이전 버전의 OS들은 이모지 누락. 이를 해결하기 위한 솔루션
    - font-variant-emoji 에 폴백 이모지 폰트 추가하기
    - 오픈 소스 color emoji 사용하기

### **[WordPress Playground](https://developer.wordpress.org/playground/)**

- 워드프레스 플레이그라운드 제공
    - PHP는 WASM으로(Emscripten) 실행
    - MySQL은 워드프레스 플러그인을 통해 SQLite로 대체. MySQL 쿼리를 인터셉트하여 SQLite로 재작성
    - 웹 서버는 서비스 워커로 구현
    - 네트워킹은 웹소켓
- [https://web.dev/wordpress-playground/](https://web.dev/wordpress-playground/)

### **[Wix’s new tool can create entire websites from prompts](https://techcrunch.com/2023/07/17/wixs-new-tool-can-create-entire-websites-from-prompts/)**

- Wix에서 AI Site Generator 출시.
- Wix의 도메인 전문 지식과 AI에 대한 경험을 활용하여 고품질 콘텐츠, 맞춤형 레이아웃 제공

### **[Excellence is a habit, but so is failure](https://awesomekling.github.io/Excellence-is-a-habit-but-so-is-failure/)**

- 조금씩 점진적으로 개선하면 큰 성과를 얻는 것처럼, 점진적인 방치와 실수는 축적되어 부정적인 결과로 이어짐.