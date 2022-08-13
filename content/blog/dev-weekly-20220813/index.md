---
title: dev-weekly 2022-08-13
date: "2022-08-13T17:00:00.000Z"
description: "dev-weekly 2022-08-13"
tags: ["javascript", "node", "css"]
---

# CSS

### **[How I Added Scroll Snapping To My Twitter Timeline](https://css-tricks.com/how-i-added-scroll-snapping-to-my-twitter-timeline)**

- scroll-snap이 캐러셀 등의 x축 뿐 아니라 y측에 적용했을 때 얻는 유용함
- 뷰포트보다 큰 컨텐츠에서의 이슈 및 브라우저별 구현이 상이한 이슈

# Node

### **[No More 'Native Modules' for Node.js. Sort of.](https://github.com/nodejs/node/pull/44135)**

- 이제 Native Modules 이라는 용어 대신, built-in module, addon 사용

### **[Sync Scroll: A VS Code Extension to Scroll Split Panes Simultaneously](https://marketplace.visualstudio.com/items?itemName=dqisme.sync-scroll#syncscroll)**

- VSCode 익스텐션. 하나의 파일에서 스크롤을 하면 다른 파일의 싱크를 맞춰서 스크롤.

### Release

- [fastify 4.4.0](https://github.com/fastify/fastify/releases/tag/v4.4.0)
- [prisma 4.2.0](https://github.com/prisma/prisma/releases/tag/4.2.0)

# Javascript

### **[Astro 1.0: The Fast Islands-Based Frontend Framework](https://astro.build/blog/astro-1/)**

- Astro 1.0 릴리즈 - 콘텐츠 중심의 빠른 웹사이트 구축을 위한 도구

### **[Patterns.dev: Modern Web App Design Patterns](https://www.patterns.dev/)**

- 모던 웹 앱의 디자인 패턴 이라는 무료 책
- 디자인 패턴, 렌더링 패턴, 성능 패턴으로 카테고라이징 되어있고, 상세한 내용과 많음 참조가 들어간 고퀄리티 서비스

### **[TypeScript 4.8 is now in release candidate stage.](https://devblogs.microsoft.com/typescript/announcing-typescript-4-8-rc/)**

- `--build`, `--watch`, `--incremental` 성능 향상

### Release

- [playwright 1.25.0](https://github.com/microsoft/playwright/releases/tag/v1.25.0)
- [lerna 5.4.0](https://github.com/lerna/lerna/releases/tag/v5.4.0)

### **[Code Golfing Tips and Tricks for Smaller JavaScript Code](https://getbutterfly.com/code-golfing-tips-tricks-how-to-minify-your-javascript-code/)**

- 코드 골프란 멋진 일을 하기 위해 가장 적은 양의 코드를 쓰는 것
- 능력 테스트이므로 일반 코드에선 사용하면 안됨
- ex) `var a=8,b=13;a=[b,b=a][0]`

### **[Size Limit 8.0: Performance Budgeting Tool for JavaScript](https://github.com/ai/size-limit)**

- performance budget tool. CI의 커밋들을 확인하고 엔드 유저에게 딜리버리 될 JS 용량을 계산해 한도를 초과하면 pull request에 에러를 표시