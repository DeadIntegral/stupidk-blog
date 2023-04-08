---
title: dev-weekly 2022-12-10
date: "2022-12-10T19:30:00.000Z"
description: "dev-weekly 2022-12-10"
tags: ["javascript", "css", "node"]
---

# CSS

### **[State of CSS 2022](https://2022.stateofcss.com/en-US/)**

- [stateofcss.com](http://stateofcss.com) 에서는 comming soon이라고 나오지만 직접 접근 가능

### **[Accessible Front-End Patterns For Responsive Tables](https://www.smashingmagazine.com/2022/12/accessible-front-end-patterns-responsive-tables-part1/)**

- 테이블을 반응형으로 만들기 위한 보편적인 솔루션은 없고, 목적에 따라 달라짐
- 반응형 테이블을 만들기 위한 관심사
    - 디자인과 시각적인 부분
    - ARIA Role
    - 접근성 친화적인 제목(caption)
    - 그라데이션을 통해 스크롤 가능하다는 인디케이트 주기
    - sticky 헤더

# Node!

### **[New npm Features for Secure Publishing and Safe Consumption](https://github.blog/2022-12-06-new-npm-features-for-secure-publishing-and-safe-consumption/)**

- npm 패키지 생태계를 위해 `세분화된 액세스 토큰`과 `코드 탐색기` 기능 추가
    - [https://docs.npmjs.com/about-access-tokens](https://docs.npmjs.com/about-access-tokens)
    - 본래 유료 기능이었던 code explorer 무료로 변경

### **[Is Prisma Better Than Your 'Traditional' ORM?](https://practica.dev/blog/is-prisma-better-than-your-traditional-orm/)**

- 기존의 ORM들과 프리즈마의 공통점 및 TS로 인해 겪는 어려움등에 대한 소개
- 컨셉별로 프리즈마가 다른 ORM들과 다른 점에 대해 상세한 설명

### **[40+ Node.js Integration Test Best Practices](https://github.com/testjavascript/nodejs-integration-tests-best-practices)**

- Nodejs에서 통합 테스트에 대해 각 구간(컨셉)에 대한 설명 및 예제코드 제공

### **[chatgpt-api: A Node Client for ChatGPT](https://github.com/transitive-bullshit/chatgpt-api)**

- 비공식 GPT-3기반 ChatGPT API Nodejs client

### **[Odiff: A Fast Pixel-by-Pixel Image Diffing Tool and Library](https://github.com/dmtrKovalenko/odiff)**

- 두 이미지의 다른 부분을 픽셀 단위로 추출하여 시각적으로 표현해주는 도구

# Javascript

### **[Vite 4.0 Released](https://vitejs.dev/blog/announcing-vite4.html)**

- 3 출시 이후 5개월만에 Vite 4.0 릴리즈. 커진 생태계에 대한 간략한 소개
- 개발모드에서 SWC를 사용하는 React 플러그인 추가
    - **`@vitejs/plugin-react`**, **`@vitejs/plugin-react-swc (new)`**
- 브라우저 컴팻 최소 사파리14, 패키지 크기 감소

### **[Console Ninja: `console.log` Output Right Next to Your Code](https://console-ninja.com/)**

- console log를 에디터의 해당 코드 옆에 즉시 보여주는 vscode 확장

### **[Sandboxing with Partytown](https://weston.ruter.net/2022/11/30/sandboxing-with-partytown/)**

- 파티타운의 샌드박싱은 신뢰할 수 없는 타사 코드를 안전하게 실행할 만큼 강력하지 않음
- 파티타운은 프록시를 통해 브라우저 API 사용

### **Release**

- **[Announcing Rome v11](https://rome.tools/blog/2022/12/06/rome11/)**
- **[storybook v7.0.0-beta.0](https://github.com/storybookjs/storybook/releases/tag/v7.0.0-beta.0)**
- **[Nx 15.3 — Standalone Projects, Vite, Task Graph and more!](https://blog.nrwl.io/nx-15-3-standalone-projects-vite-task-graph-and-more-3ed23f7827ed)**
- **[Bun v0.3.0](https://bun.sh/blog/bun-v0.3.0)**
- **[Partytown 0.7.3](https://github.com/BuilderIO/partytown/releases/tag/v0.7.3)**
- **[React Tooltip 5.0](https://github.com/ReactTooltip/react-tooltip/releases/tag/v5.0.0)** - float ui 기반으로 변경

# Etc

### **[**VSCode November 2022 (version 1.74)**](https://code.visualstudio.com/updates/v1_74)**

- 탐색기 autoreavel 설정 (설정에 넣으면 exclude)
- 디버깅에서 console.profile 을 통한 cpu, heap profile 제공
- return 에서 go to definition 제공