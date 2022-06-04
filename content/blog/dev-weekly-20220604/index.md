---
title: dev-weekly 2022-06-04
date: "2022-06-04T14:00:00.000Z"
description: "dev-weekly 2022-06-04"
tags: ["javascript", "css", "node"]
---

# CSS

### **[Star Wars Scene Transition Effects in CSS](https://codersblock.com/blog/star-wars-scene-transition-effects-in-css)**

- `mask-image` 를 사용해서 장면 간 전환에 애니메이션 넣기
- 사용자 정의 프로퍼티를 이용한 애니메이션

### **[Don’t Fight the Browser Preload Scanner](https://web.dev/preload-scanner)**

- 브라우저가 렌더링 차단 리소스를 만났을 때 preload scanner는 계속 dom을 탐색하고, 이미지와 같은 요소들을 병렬로 요청
- preload scanner를 망가뜨리는 예제들과 수정 방법
    - js로 인라인 스크립트 삽입할 때의 이슈
    - 리소스 우선순위에 따른 트래픽 경합(bandwidth contention)
    - background-image와 같은 CSS property는 CSSOM 구성 이후 요청

### **[Pure CSS/SVG Tic Tac Toe](https://codepen.io/jh3y/pen/KKNwpzN)**

- CSS, HTML만 사용해서 만든 Tic Tac Toe 게임

# Node

### **[npm Security Update: What GitHub Learnt About April's Attack](https://github.blog/2022-05-26-npm-security-update-oauth-tokens/)**

- 2022년 6월2일자로, Github은 남용된 토큰의 모든 주인에게 통지 완료

### **[How We Converted Our Node.js Library to Deno (using Deno)](https://www.edgedb.com/blog/how-we-converted-our-node-js-library-to-deno-using-deno)**

- 런타임 어댑터 패턴을 사용하여 Deno 가 호환되는 Nodejs 라이브러리로 변경하기

### **[HTTP Testing with Hurl in Node.js](https://blog.humphd.org/http-testing-with-hurl-in-node-js/)**

- Http + Curl 에서 이름 딴 Hurl이라는 http testing 도구
- 심플한 문법과 싱글 바이너리 파일이라는 장점

# Javascript

### **[Angular v14 Released](https://blog.angular.io/angular-v14-is-now-available-391a6db736af)**

- 앵귤러 14 릴리즈
- standalone:true, CLI 자동완성, 개발도구 파이어폭스 지원, 실험적인 esbuild 기반 컴파일

### **[Compiling a Subset of JavaScript to ARM Assembly in Haskell](https://www.micahcantor.com/blog/js-to-asm-in-hs/)**

- 하스켈로 JS 서브셋을 ARM 어셈블리로 컴파일하기
- x86 대신에 ARM인 이유는 단순하기 때문에.

### **[Shaka Player 4.1: Library for Playing Adaptive Media](https://github.com/shaka-project/shaka-player)**

- DASH, HLS를 지원하는 JS 미디어 플레이어
- IndexedDB를 통한 오프라인 미디어 재생 가능

### **[Terser: JavaScript 'Mangler' and Compressor Toolkit for ES6+](https://try.terser.org/)**

- terser [https://try.terser.org/](https://try.terser.org/) 온라인 플레이 그라운드 출시