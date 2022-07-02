---
title: dev-weekly 2022-07-02
date: "2022-07-02T20:30:00.000Z"
description: "dev-weekly 2022-07-02"
tags: ["javascript", "css", "node"]
---

# CSS

### **[Single Element Loaders: The Bars](https://css-tricks.com/single-element-loaders-the-bars)**

- 하나의 요소(엘리먼트)를 사용하여 만드는 로딩 인디케이터 - 막대 모양

### **[3 Useful CSS Hacks](https://www.youtube.com/watch?v=MywezIxlp8Y)**

- vmax를 사용한 css 트릭들
- `border-radius: 100vmax;` 항상 양 옆만 50%인 모양을 유지
- `box-shadow: 0 0 0 100vmax rgb(0, 0, 0, 0.5)` backdrop 배경을 만들어주는 트릭
- `clip-path: inset(0, -100vmax);` 위와 같이 사용하면 래퍼를 무시하고 수평을 채울 수 있는 트릭

# Node

### **[Working with the File System from Node.js](https://2ality.com/2022/06/nodejs-file-system.html)**

- Node에서 파일 읽기, 쓰기, 스트림, 버퍼, 디렉토리 조작, End Of Line 등 텍스트 파일 작업과 관련된 것들에 대한 설명글 feat. DR. Axel

### **[Should Node.js Directly Support Web Workers?](https://github.com/nodejs/node/issues/43583)**

- 노드 코어에서 WebWorker support 해달라는 신드레의 제안(deno는 이미 지원)
- worker thread API는 여러면에서 다르며 제대로 연결하기 어려움.

### **[Prisma 4.0 Released: The Next Gen ORM](https://github.com/prisma/prisma/releases/tag/4.0.0)**

- 프리즈마 4.0 릴리즈
- [업그레이드 가이드](https://www.prisma.io/docs/guides/upgrade-guides/upgrading-versions/upgrading-to-prisma-4)

### BRIEF RELEASES

- [fastify v4.2.0](https://github.com/fastify/fastify/releases/tag/v4.2.0)
- **[Kafka.js 2.1](https://github.com/tulios/kafkajs/releases/tag/v2.1.0)**
- [pnpm 7.4](https://github.com/pnpm/pnpm/releases/tag/v7.4.1)
- [ioredis 5.1](https://github.com/luin/ioredis/releases/tag/v5.1.0)

# Javascript

### **[Vercel Edge Functions](https://vercel.com/changelog/vercel-edge-functions-are-now-in-public-beta)**

- Vercel Edge Functions 퍼블릭 베타
- [https://vercel.com/docs/concepts/functions/edge-functions](https://vercel.com/docs/concepts/functions/edge-functions)

### **[Next.js 12.2](https://github.com/vercel/next.js/releases/tag/v12.2.0)**

- Next v12.2 release
- [https://nextjs.org/blog/next-12-2](https://nextjs.org/blog/next-12-2)

### **[Retry XMLHttpRequest Carefully](https://lofi.limo/blog/retry-xmlhttprequest-carefully)**

- 안전하게 요청을 다시 보내는 방법
- Automatic Retry의 개념에서 시작해서 Delayed Retry, Exponential Backoff, Too Important to Be Left to Chance, Bringing it Together 에 걸쳐 개선해나가는 아티클

### **[Vue 2.7 'Naruto' Released](https://blog.vuejs.org/posts/vue-2-7-naruto.html)**

- Vue 2.7 릴리즈. 뷰2는 2023년 EOL 에 도달하지만 2 사용자를 위한 LTS 버전