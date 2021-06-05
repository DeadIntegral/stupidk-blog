---
title: dev-weekly 2021-06-05
date: "2021-06-05T10:10:00.000Z"
description: "dev-weekly 2021-06-05"
tags: ["javascript", "node"]
---

# Node

### [Electron 13.0 Released](https://www.electronjs.org/blog/electron-13-0)

- 크롬 90, 91, 노드 14, 14.16.0, v8 9.0, 9.1 적용
- new-window WebContents로 대체
- Electron 10.xy 지원 종료

### [Node v16.3.0 (Current) Released](https://nodejs.org/en/blog/release/v16.3.0/)

- 다양한 버그 수정, 종속성 업데이트
- npm install 에 workspace 지원

- Node 15 EOL - 노드15 죽음
    - [https://github.com/nodejs/Release](https://github.com/nodejs/Release)
- stackoverflow $1.8B 인수
    - [https://github.com/nodejs/Release](https://github.com/nodejs/Release)

# Javascript

### [Making JavaScript Run Fast on WebAssembly](https://bytecodealliance.org/articles/making-javascript-run-fast-on-webassembly)

- WASM으로 만든 JS 엔진
- JS 엔진이 제공되지 않거나 JIT을 제공하지 않는 플랫폼을 위한 WASM JS Engine
- 서버리스 환경의 경우 콜드 스타트 시점에 js가 뜨기까지 5밀리초의 시간이 걸리는데, 이를 무효화([https://github.com/bytecodealliance/wizer](https://github.com/bytecodealliance/wizer) 라는 도구를 이용, 13배 빠른 스타트)

### [Svelte for the Experienced React Dev](https://css-tricks.com/svelte-for-the-experienced-react-dev/)

- 리액트의 각 컨셉들을 스벨트에서 어떻게 사용하는지 비교하여 설명

### Quick Bits

### [https://blog.chromium.org/2021/06/chrome-92-web-apps-as-file-handlers-new.html](https://blog.chromium.org/2021/06/chrome-92-web-apps-as-file-handlers-new.html)

- 크롬 92 베타
- 파일 핸들링 API
- size-adjust Descriptor for @font-face - font glyph 조정 가능

### [https://developer.chrome.com/blog/new-in-devtools-92/](https://developer.chrome.com/blog/new-in-devtools-92/)

- 크롬 92 개발자 도구
- 크롬 콘솔에서 const 재선언 가능
- 그리드 에디터
- CORS 디버깅 - 왜 CORS가 발생했는지 원인 표시

## Articles, Opinions & Tutorials

### [An Introduction to WebAssembly for JavaScript Developers](https://pascalpares.appspot.ovh/webassembly-for-javascript-developers/)

- JS에서 WASM 을 어떻게 사용하는지 기초 포스트
- 다음과 같이 메모리 잡히는 부분까지 디테일하게 설명

    ```jsx
    Offsets|       Bytes       | Array Entries
    ----------+-------------------+----------------------
            0 |0x01 0x00 0x00 0x00| a[0]
            4 |0x02 0x00 0x00 0x00| a[1]
            8 |0x03 0x00 0x00 0x00| a[2] 
           12 |0x41 0x42 0x43 0x44| b[0] b[1] b[2] b[3]
           16 |0x45 0x46 0x00 0x00| b[4] b[5] 0x00 0x00
           20 |0x04 0x00 0x00 0x00| c[0]
           24 |0x05 0x00 0x00 0x00| c[1]
    ```

### [How to Use Pivot Tables with SpreadJS](https://www.grapecity.com/blogs/how-to-use-pivot-tables-with-spreadjs)

- spreadjs 14.10 릴리즈.
- spreadjs 에서 피벗 테이블 사용하기 아티클

## Code & Tools

### [PLV8 3.0: V8 JavaScript, But for Postgres](https://github.com/plv8/plv8)

- V8 엔진으로 구동되는 PostgreSQL procedural language 제공하는 공유 라이브러리

### [Svelte-Motion: Animation Library for Svelte based on Framer Motion](https://svelte-motion.gradientdescent.de/)

- Framer Motion을 기반으로 한 Svelte animation 라이브러리