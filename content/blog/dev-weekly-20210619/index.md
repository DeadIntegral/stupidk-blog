---
title: dev-weekly 2021-06-19
date: "2021-06-19T19:00:00.000Z"
description: "dev-weekly 2021-06-19"
tags: ["javascript", "node", "CSS"]
---

# CSS, Node

### [CSS for Web Vitals](https://web.dev/css-web-vitals)

- 레이아웃, 이미지, 폰트, 애니메이션의 보다 나은 사용 방법
- feat. [CLS](https://web.dev/cls/), LCP, FOUT, [high Performance Animation](https://web.dev/animations/)

웹 접근성을 준수한다면, colour contrast analyser 도 맞춰야 함

[https://webaim.org/resources/contrastchecker/](https://webaim.org/resources/contrastchecker/)

## Node

### [A Visual Guide to Node.js Streams](https://blog.insiderattack.net/a-visual-guide-to-nodejs-streams-9d2d594a9bf5)

- 스트림에 대한 개념을 그림을 이용해서 쉽게 설명한 포스트

### [Next.js 11 Released](https://nextjs.org/blog/next-11)

- Improved Performance - cold startup time
- webpack5
- `next/script`, `next/image` - `<Script />`, `<Image />`
- CreateReactApp Migration tool(experimental)
- Nextjs live - 빌드없이 url을 공유하여 다른 사람들과 공동작업

### [A Beginner's Guide to the File System Module (fs)](https://catalins.tech/a-beginners-guide-to-the-file-system-module-in-nodejs)

- fs module 개념, 동기(접미사 Sync)와 비동기, path
- writeFile, readFile, readdir, unlink, mkdir, rmdir, rename, appendFile

# JavaScript

### [Benchmarking JavaScript Memory Usage](https://blog.webpagetest.org/posts/benchmarking-javascript-memory-usage/)

- 웹브라우저에서의 자바스크립트 메모리에 대하여
- 웹에서 메모리 할당의 35%는 js, 10%는 DOM
- 라이브러리(프레임워크)별 초기 메모리 사용량과 그 효율

## Quick Bits

### [https://v8.dev/features/import-assertions](https://v8.dev/features/import-assertions)

- json 파일을 import할 때 mime타입에 따라 악성 제공자의 스크립트가 실행될 수 있음
- 아래와 같이 요청할 경우 타입이 json이 아니면, 권한 상승이 이루어지지 않고 import 실패

    ```jsx
    import data from 'https://evil.com/data.json' assert { type: 'json' };
    ```

- dynamic import에서도 사용 가능

    ```jsx
    const jsonModule = await import('./foo.json', {
      assert: { type: 'json' }
    });
    ```

### [https://deno.com/blog/v1.11](https://deno.com/blog/v1.11)

- deno 1.1 릴리즈
- Official Docker images : alpine, centos, debian (default), distroless, ubuntu
- stable한 deno lint : eslint보다 100% 빠르다고 함
- BroadcastChannel : 웹워커간 메시지를 브로드캐스트 하기 위한 브라우저 API 지원

## Articles, Opinions & Tutorials

### [When CSS Isn’t Enough: JavaScript Requirements For Accessible Components](https://www.smashingmagazine.com/2021/06/css-javascript-requirements-accessible-components/)

- CSS Hack을 통해 only CSS로 구현했을 때 발생하는 웹 접근성 이슈들
- Toolip, Modal, Tab, Carousel, Dropdown Menu

## Code & Tools

### [MathJax 3.2.0: Beautiful Math Rendering in All Browsers](https://www.mathjax.org/)

- 모든 브라우저에서 작동하는 수학 디스플레이 js 엔진
- 다음과 같이 $$ 사이에 TeX를 입력하면 적용

    ```jsx
    $$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$
    ```

- 웹 폰트, svg 사용을 통한 확대/축소 대응

### [A Pathfinding Algorithm Visualizer](https://josephprichard.github.io/Pathfinder/)

- 경로탐색 알고리즘 시각화
- 클릭, 드래그 등을 통하여 장애물, 가중치 등을 설정가능