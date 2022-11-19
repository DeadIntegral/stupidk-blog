---
title: dev-weekly 2022-10-29
date: "2022-10-29T11:00:00.000Z"
description: "dev-weekly 2022-10-29"
tags: ["javascript", "css", "node", "devtool"]
---
# CSS

### **[100 Days Of More Or Less Modern CSS](https://www.matuzo.at/blog/2022/100-days-of-more-or-less-modern-css)**

- 최신 CSS 사용 가이드
- var() fallback, inline-start,end, subgrid, max() trick, ::backdrop 등

### **[Futuristic CSS](https://www.smashingmagazine.com/2022/10/futuristic-css)**

- 언젠가 브라우저에 적용될 수 있는 CSS 살펴보기
- Toggle(chrome v108지원), Switch Function, Intrinsic Typography, Sibling Functions, Patterns 등

### **[Radix UI](https://www.radix-ui.com/)**

- UI 컴포넌트 라이브러리

# Node

### **[route-list: CLI Tool to Display Express/Koa/Hapi/Fastify Routes](https://github.com/VladimirMikulic/route-list)**

- Express, Koa, Hapi, Fastify 등에서 route list를 콘솔에 이쁘게 출력하는 도구

### **[Node 18 Becomes Active LTS with v18.12.0](https://nodejs.org/en/blog/release/v18.12.0/)**

- Node 18.12.0 릴리즈 및 “Active LTS”로 전환. 코드명 Hydrogen

### **[npm 9.0.0 Released](https://github.blog/changelog/2022-10-24-npm-v9-0-0-released/)**

- npm 9.0.0 릴리즈.
- semver update `^14.17.0 || ^16.13.0 || >=18.0.0`

# Javascript

### **[Next.js 13 Unveiled at Next.js Conf](https://nextjs.org/blog/next-13)**

- `app/` directory
    - layout RFC에서 언급했던대로 디렉토리 구조 변경. next13에서는 기존 구조도 지원.
    - layout 기능을 layout파일로 대체.
    - loading.js를 통한 suspense - layout.js를 먼저 렌더링하고, loading.js를 보여주다가 데이터가 로드되면 본래 page를 표시
- Turbopack (alpha) - 웹팩 대체
- `next/image` 향상 - srcset생성, priority 요소 제공 등
- `next/font` 새로운 폰트 시스템 - CSS, font 파일은 빌드 시 다운로드되어 브라우저가 외부에 요청하지 않음
- `next/link` - a 태그로 래핑하지 않아도 되게 변경 (자동으로 변경해주는 도구 지원)
- OG image genderation - 동적으로 og image를 생성하고 vercel edge function을 이용
- 미들웨어 API 업데이트, React 최소버전 18.2.0, Nodejs 최소버전 14.6.0, IE지원 제거 등

### **[Babel 7.20.0](https://babeljs.io/blog/2022/10/27/7.20.0.html)**

- TS 4.9 지원, deno 컴파일 타겟 설정 지원, 바벨로더 9.0

### **[Deno 1.27](https://deno.com/blog/v1.27)**

- language Server/IDE 향상 - 자동완성 레지스트리
- API들 안정화, lint 업데이트, v8 10.8 적용, Nodejs 호환성 개선 등

### **[Which Serverless Edge Platform Has the Fastest Git Deployments?](https://deno.com/blog/fastest-git-deploys-to-the-edge)**

- Edge 플랫폼들 배포 속도 비교
- deno가 가장 빠름 - VM, Docker container 대신에 v8 isolate를 사용했기 때문

### **[How to Build a Blog with Fresh and Deno](https://deno.com/blog/build-a-blog-with-fresh)**

- Fresh 로 블로그를 구축하는 예제

### **[Canvas Confetti: An On-Demand Confetti Shower](https://www.kirilv.com/canvas-confetti/)**

- 색종이 총 이펙트 도구.
- 여러 이펙트를 동시에 발동해도 하나의 캔버스만 존재.

# DevTools

### **[What’s New In DevTools: Halloween Edition](https://www.smashingmagazine.com/2022/10/devtools-updates-halloween-edition)**

- 브라우저들의 개발자 도구 리뉴얼
    - 크롬 - 102부터 새롭게 지원하는 Performance Insight
    - 파이어폭스
        - cpu, event loop, 그래픽, 브라우저 단의 stack등 디테일한 영역까지 전부 프로파일링해주는 새 도구(단축키: ctrl + shift +1, 2)
        - 네트워크 탭에서 요청 edit and resend 기능
        - 이벤트 리스너 on, off 기능 추가
    - 엣지 - 네트워크 탭의 Fulfilled by 항목 추가. 서비스 워커, PWA 디버깅 지원