---
title: dev-weekly 2022-08-27
date: "2022-08-27T12:00:00.000Z"
description: "dev-weekly 2022-08-27"
tags: ["javascript", "node", "css"]
---

# CSS

### **[Use the Right Container Query Syntax](https://www.oddbird.net/2022/08/18/cq-syntax)**

- 컨테이너 쿼리 사용 시 주의할 점(무한루프, 브라우저 지원 등)

### **[Using :has() as a CSS Parent Selector and Much More](https://webkit.org/blog/13096/css-has-pseudo-class)**

- :has() 의 탄생 배경 및 브라우저 컴팻 상황
- :has() 의 다양한 가능성 (다른 셀렉터와 조합해서 사용하는 예제들)

### **[CSS Grid and Custom Shapes, Part 2](https://css-tricks.com/css-grid-and-custom-shapes-part-2)**

- Part1과 마찬가지로 grid, clip-path, mask로 작업
- 중첩된 이미지 그리드
- 이미지 패널 확장

### **[Quick Tip: Negative Animation Delay](https://css-irl.info/quick-tip-negative-animation-delay)**

- animation delay를 음수로 할당하여 즉시 실행하는 팁

### **[An Interactive Guide To Color & Contrast](https://colorandcontrast.com/#/)**

- 색상과 대비에 대한 인터렉티브 가이드
- 눈(각막, 동공, 홍채, 렌즈, 망막) 부터 시작하여 색각, 대비 시력, 감각 적응, 색 모델에 이르기까이 광범위한 영역에 대한 가이드

### **[Single Div Stapler](https://codepen.io/kassandrasanch/pen/yLOOgNy)**

- 하나의 div에 CSS로 페인팅한 스테이플러

# Node

### **[Popular Node.js Patterns and Tools to Reconsider?](https://practica.dev/blog/popular-nodejs-pattern-and-tools-to-reconsider/)**

- 다시 한번 생각해봐야할 노드의 패턴들 - 잘못될 수 있는 이유와 보다 나은 대안

### ****[Big Changes Ahead for Deno](https://deno.com/blog/changes)****

- 노드와 NPM 모듈 호환 - 3개월 이내 90% 목표
- 가장 빠른 JS런타임. 다음 릴리즈에 포함할 새로운 HTTP 서버는 가장 빠른 JS 웹 서비스

### **[file-type 18.0: Detect the File Type of a Buffer, Uint8Array or ArrayBuffer](https://github.com/sindresorhus/file-type)**

- 로우 데이터를 제공하면 파일을 디텍트 해주는 도구.
- 매직넘버를 사용하기 때문에 Buffer/Uint8Array/ArrayBuffer 파일 타입 감지

### **[Soketi: Simple and Fast WebSockets Server](https://github.com/soketi/soketi)**

- Cloudflare worker에 배포할 수 있는 서버리스 웹소켓

### **[brotli-wasm: A Reliable Brotli Compressor and Decompressor](https://github.com/httptoolkit/brotli-wasm)**

- WASM을 통해 노드와 브라우저를 지원하는 Compressor

# Javascript

### [Creator of Bun Forms Oven](https://oven.sh/)

- Bun 에서 회사 설립 Oven

### **[TypeScript 4.8 Released](https://devblogs.microsoft.com/typescript/announcing-typescript-4-8/)**

- TS 4.8 릴리즈

### [How do you pronounce JSON?](https://www.notion.so/2022-08-27-f53b6084afc14d60bdfddae0090ea757)

- JSON의 창시자 더글라스 크락포드에게 JSON의 발음 물어본 영상
- 본인은 Jason이라고 읽었고, 사람들이 Jay-sawn 이라고 읽지만 괜찮다고 함

### [Storybook 7.0 Alpha](https://storybook.js.org/blog/7-0-design-alpha/)

- 레이아웃 변경
- CSS와 정렬을 디버깅 하기 위한 툴바 제공
- 200개 이상의 새로운 아이콘
- 성능을 위한 pre-bundle과 종속성 충돌 제거

### **[Understanding When and Why React Re-Renders](https://www.joshwcomeau.com/react/why-react-re-renders/)**

- 리액트가 왜 리렌더링 되는지에 대한 상세한 글