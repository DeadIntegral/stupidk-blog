---
title: dev-weekly 2023-04-22
date: "2023-04-22T10:00:00.000Z"
description: "dev-weekly 2023-04-22"
tags: ["javascript", "css", "node", "infra", "etc"]
---
# Node

### **[Node.js 20 Released](https://nodejs.org/en/blog/announcements/v20-release-announce)**

- Nodejs 권한 모델 - 실행 중 특정 리소스에 대한 액세스를 제한하기 위한 메커니즘
- 안정적인 test runner
- V8 엔진 11.3 업데이트
- 윈도우에서 ARM64 공식 지원
- Ada 2.0(Url parser) 업데이트

### **[AdminJS 7.0 is an admin panel for apps written in node.js](https://docs.adminjs.co/installation/whats-new-in-v7)**

- AdminJS 7.0 릴리즈.
- ESM Only 호환, 로그인 페이지 SPA, 디자인 시스템 업데이트

# CSS

### **[Solving the CSS layout and source order disconnect](https://developer.chrome.com/blog/reading-order/)**

- css order 등으로 UI가 변경되더라도 스크린 리더는 소스에 배치된 순서대로 읽는 이슈
- `reading-order: auto;` 라는 프로퍼티로 해결하려는 CSS Woking Group의 제안

# Javascript

### **[Optimizing resource loading with the Fetch Priority API](https://web.dev/fetch-priority/)**

- 리소스 우선순위에 대한 개념 설명 및 `fetchpriority` 프로퍼티 소개
- 상대적 우선순위 및 사용사례 설명
- fetchpriority 는 지시문이 아니라 힌트. 충돌이 발생하면 브라우저가 필요하다고 간주되는 것이 우선적용될 수 있음. (preload는 힌트가 아니라 강제)
- 크롬 102+, 엣지 102+. 아직 그 외 브라우저에서 사용 불가

### **[Interaction to Next Paint (INP): What is it and How to Improve It](https://calibreapp.com/blog/interaction-to-next-paint)**

- INP는 페이지가 방문자 인터랙션을 얼마나 잘 처리하는지 평가하는 지표. 이 지표에 대한 설명, 추적하는 법, 향상시키는 법 등.
    - 사용자의 액션 후 다음 페인트까지 걸리는 시간
    - 백분위 98 을 사용하기 때문에 메트릭이 왜곡되지는 않을 것.
- 좋은 INP 측정에 대한 설명 - 구글 가이드라인에서는 200ms 미만
- 주의사항 - 사용자의 디바이스나 인터넷 연결 상태로 인한 영향

### **[Vite 4.3 is out!](https://vitejs.dev/blog/announcing-vite4-3.html)**

- 리액트 컴포넌트 1000개에 대해서 Vite 4.2 대비 20~70% 개선.
    - babel, swc 별 콜드 스타트, 웜 스타트, 루트 HMR, Leaf HMR 별 성능 비교
- [https://sun0day.github.io/blog/vite/why-vite4_3-is-faster.html](https://sun0day.github.io/blog/vite/why-vite4_3-is-faster.html) 4.3 이 빠른 이유
    - 4.2까지는 중복 resolve logic, 불필요한 모듈 검색이 많았는데 이를 개선.

### **[Announcing TypeScript 5.1 Beta](https://devblogs.microsoft.com/typescript/announcing-typescript-5-1-beta/)**

- 정의되지 않은 함수에 대한 더 쉬운 암시적 변환
- `@param` JSDoc Tag에 대한 자동 완성
- JSX 지원 향상
- 최적화
- 브레이킹 체인지 - 최소사양 ES2020, Nodejs14.17

# Etc

### **[Load Balancing](https://samwho.dev/load-balancing/)**

- 단일 로드 밸런서가 HTTP 요청을 서버 인스턴스들에게 분배하는 방법에 대한 설명글
- 가장 베이직한 컨셉부터 최신 알고리즘까지 시각화하여 표현

### **[Passkeys: What the Heck and Why?](https://css-tricks.com/passkeys-what-the-heck-and-why/)**

- passkey와 WebAuthn(FIDO2) 에 대한 설명 - passkey 는 WebAuthn위에 구축된 사양
- passkey는 자격 증명의 클라우드 동기화, WebAuthn은 단일 장치 자격 증명

### **[I Made My Blog Solar-Powered, Then Things Escalated](https://louwrentius.com/i-made-my-blog-solar-powered-then-things-escalated.html)**

- 태양광 패널로 전기를 생산하고, 라즈베리 파이를 통해 블로그 운영하기

### **[대체불가능한 개발자가 되는 법 - 존 카맥](https://www.youtube.com/watch?v=CMv8LzuuTKk)**

- 프로그래밍의 핵심은 유저들에게 가치를 제공하는 것.
- 가치가 무엇인가에 대해서는 논쟁이 있겠지만, 유저가 제품에 실망했다면 ‘가치’를 만들어내지 못한 것.
- 우리가 알지 못하는 작은 시장도 존재 할 것. 하지만 우리는 실질적으로 존재하는 유저를 타겟으로 잡아야 하고, 이들에게 맞는 제품을 만들려고 노력 해야 함. 가상의 유저를 만들어내지 말 것.