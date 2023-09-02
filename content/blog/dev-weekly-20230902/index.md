---
title: dev-weekly 2023-09-02
date: "2023-09-02T17:35:00.000Z"
description: "dev-weekly 2023-09-02"
tags: ["javascript", "node", "css"]
---

# CSS

### **[CSS Selectors: A Visual Guide](https://fffuel.co/css-selectors)**

- CSS 셀렉터들이 어떤걸 선택하는지 시각화한 자료

### **[CodePen Home Solar Eclipse](https://codepen.io/ykadosh/pen/GRwLKvV)**

- 이미지 없이 HTML, CSS만 사용해서 만든 일식

# Node

### **[The complexity of writing an efficient NodeJS Docker image](https://www.specfy.io/blog/1-efficient-dockerfile-nodejs-in-7-steps)**

- 효율적인 NodeJS Docker이미지 만들기 스텝 바이 스텝
- dockerignore, slim, multi stage build(노드 모듈 제거), 캐시 종속성, devDependency 제거 등
    - alpine은 glibc대신 msul libc로 작동하고, segfault 이슈가 있음

### **[Creating an NPX tool](https://nayte.dev/posts/creating-an-npx-tool/)**

- NPX 패키지 만들기 샘플 (헬로 월드)

# Javascript

### **[Use web components for what they’re good at](https://nolanlawson.com/2023/08/23/use-web-components-for-what-theyre-good-at/)**

- [“If Web Components are so great, why am I not using them?”](https://daverupert.com/2023/07/why-not-webcomponents/)에 대한 반박글.
- 대기업의 디자인 시스템에서 많이 사용되는 중. 이들은 여러 프레임워크를 만족시켜야 하기 때문.
- 웹 컴포넌트의 단점 - SSR, 접근성 등
- 필요하면 사용하는 것. 브라우저 벤더사에게 아웃소싱 한다는 강점 존재.

### **Release**

- [Prisma 5.2](https://github.com/prisma/prisma/releases/tag/5.2.0)
- [Axios 1.5](https://github.com/axios/axios/releases/tag/v1.5.0)
- [pnpm 8.7](https://github.com/pnpm/pnpm/releases/tag/v8.7.0)
- [Fastify 4.22](https://github.com/fastify/fastify/releases/tag/v4.22.0)

# ETC

### **[THE IDEAL VIEWPORT DOESN’T EXIST](https://viewports.fyi/)**

- 12만개의 데이터를 확인했는데 사용되는 뷰 포트의 종류가 2300가지.
- 뷰 포트 단위로 디자인 결정을 하지 말고, 유연한 규칙을 만들라는 글.

### **[How I Write Alt Text for Code Snippets on Social Media](https://benmyers.dev/blog/code-snippet-alt-text/)**

- code snippet에 알맞는 Alt 입력하기.
- CSS는 그대로 기입, HTML 설명하기 등. 코드가 길면 링크를 제공하고 전체 코드 제공하기.

### **[Announcing the MDN front-end developer curriculum](https://developer.mozilla.org/en-US/blog/announcing-mdn-front-end-developer-curriculum/)**

- MDN에서 작성하는 프론트엔드 커리큘럼
- 2019년에 웹 개발 학습은 MDN 전체 문서 중 10% 비중. 학습 영역을 보완하는 작업.