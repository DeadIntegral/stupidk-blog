---
title: dev-weekly 2023-07-29
date: "2023-07-29T16:30:00.000Z"
description: "dev-weekly 2023-07-29"
tags: ["javascript", "css", "node"]
---
# 2023-07-29

# CSS

### **[Can We Query the Root Container?](https://www.oddbird.net/2023/07/05/contain-root/)**

- 중첩된 요소의 크기를 변경하면 컨테이너가 새 콘텐츠 크기를 적절히 포함하기 위해 리플로우 발생
- 관찰자의 역설때문에 구현이 불가능하다고 생각했었음.
- 루트 엘리먼트에 container-type: size를 입력하면 스크롤이 불가능해지는 것과 같은 브라우저 이슈들
- root, body propagation에 대하여.

# Node

### **[Node.js Best Practices: 2023 edition is here](https://github.com/goldbergyoni/nodebestpractices)**

- NodeJS 베스트 프랙티스 프로젝트가 2023년 표준으로 업데이트

### **[Introducing TypeChat](https://microsoft.github.io/TypeChat/blog/introducing-typechat/)**

- 자연어로 질문하면 JSON 데이터 포맷으로 반환하는 도구
- TypeScript 로 타입을 지정해주면, 자연어를 타입에 맞는 데이터 포맷으로 반환

### **[Bun v0.7.0](https://bun.sh/blog/bun-v0.7.0)**

- 실험적 Vite 지원
- 별도의 스레드에서 다른 JS 인스턴스를 실행할 수 있는 워커 지원
- `structuredClone`, `AsyncLocalStorage` 지원
- Nodejs 호환성 개선

### **[Proposal: Support `.env` files](https://github.com/orgs/nodejs/discussions/44975)**

- node에서 .env를 지원하는 풀 리퀘스트.
- deno, bun은 빌트인으로 지원중

### Release

- [ink v4.3.0](https://github.com/vadimdemedes/ink/releases/tag/v4.3.0)
- [jasmine 5.1.0](https://github.com/jasmine/jasmine/blob/main/release_notes/5.1.0.md)
- [Arc 1.0 release](https://start.arc.net/release-notes)
- [remix 1.19](https://github.com/remix-run/remix/releases/tag/remix%401.19.0)
- [a11y-dialog 8.0.0](https://github.com/KittyGiraudel/a11y-dialog/releases/tag/8.0.0)
- [fingerprintjs 4.0](https://github.com/fingerprintjs/fingerprintjs/releases/tag/v4.0.0)

# Javascript

### **[WebGPU: the cross-platform graphics API of tomorrow](https://developer.chrome.com/blog/webgpu-cross-platform/)**

- WebGPU 브라우저 API를 만들며 webgpu.h도 개발.
- webgpu.h를 사용하여 데스크톱 앱과 웹 모두에서 사용 가능한 단일 코드베이스 만들기
    - webgpu.h, webgpu_cpp.h 는 아직 안정화되지 않음
    - Emscripten으로 빌드(WASM)

### **[Introducing React Tweet](https://vercel.com/blog/introducing-react-tweet)**

- 성능 저하 없이 트위터 글을 임베드해주는 리액트 컴포넌트 라이브러리
- 트위터 임베드는 약 560kb인데 이 도구는 16kb

### **[Astro 2.9: View Transitions (experimental)](https://astro.build/blog/astro-290/)**

- Astro 2.9 릴리즈. 실험적인 View Transition 제공
- redirects 스테이블 지원.

### **[Good code is like a love letter to the next developer who will maintain it.](https://addyosmani.com/blog/good-code/)**

- 코드를 이쁘게 작성하라는 글.
- 우리 산출물의 아름다움은 알고리즘의 우아함이나 효율성에 의해 판단되는 것이 아니라, 다른 사람들이 우리 작업을 기반으로 구축할 수 있는 기쁨과 용이함으로 판단되는 것.

# ETC

### **[Google's next big idea for browser security looks like another freedom grab to some](https://www.theregister.com/2023/07/25/google_web_environment_integrity/)**

- WEI(Web Environment Integrity) API 제안. 클라이언트가 클라이언트의 무결성을 증명하는 토큰을 사용해 신뢰를 구축하는 방법.

### **[Over 4600 pixel-perfect icons for web design](https://tabler-icons.io/)**

- 무료 오픈소스 아이콘 모음.

### **[Shrinking VS Code with name mangling](https://code.visualstudio.com/blogs/2023/07/20/mangling-vscode)**

- VSCode의 workbench.js는 시간이 지나면서 계속 커지는 중.
- 함수의 인자 등을 mangling(일치하는 모든 이름을 의미없지만 짧은 글자로 변경하는 것)하면 용량 감소(workbench.js는 약 1메가 감소, vscode 번들 전체에서 실행하면 3.8메가 감소)
- 개런티 때문에 맹글링 하지 않는다면, TS로 맹글링하기

### **[Meta를 떠나는 댄의 소회](https://twitter.com/dan_abramov/status/1682029195843739649)**

### **[How to build a GPT-3 App with Nextjs, React, and GitHub Copilot](https://github.blog/2023-07-25-how-to-build-a-gpt-3-app-with-nextjs-react-and-github-copilot/)**

- 코파일럿을 이용해서 GPT-3 앱을 만드는 github 블로그 글.