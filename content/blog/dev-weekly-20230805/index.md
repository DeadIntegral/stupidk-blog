---
title: dev-weekly 2023-08-05
date: "2023-08-05T16:00:00.000Z"
description: "dev-weekly 2023-08-05"
tags: ["javascript", "css", "node"]
---

# CSS

### **[Randomness in CSS using trigonometry](https://hypersphere.blog/blog/randomness-in-css-using-trigonometry/)**

- CSS에 도입된 삼각함수를 이용해 만드는 애니메이션
- 사인 함수의 특성 이용하기 - 제한된 값(정규화), 연속성

### **[The virtual keyboard API](https://ishadeed.com/article/virtual-keyboard-api/)**

- 모바일에서 가상키보드가 활성화 될 때 sticky header와 sticky floating button 이슈
- VirtualKeyboard API 를 사용하여 스텝 바이 스텝으로 문제들 해결하는 과정

### **[Scroll progress animations in CSS](https://developer.mozilla.org/en-US/blog/scroll-progress-animations-in-css/)**

- `animation-timeline: scroll(root block);` 를 통해 CSS로 scroll에 바인드하기

# Node

### **[Run JavaScript/WASM in Python: high-level SpiderMonkey bindings to Python with PythonMonkey](https://medium.com/@willkantorpringle/pythonmonkey-javascript-wasm-interop-in-python-using-spidermonkey-bindings-4a8efce2e598)**

- 파이선 VM에 모질라 스파이더 몽키를 추가
- 서로의 패키지를 가능한 성능 저하 없이 원활하게 사용 가능.
- 스파이더 몽키의 WASM API 를 통해 WASM 도 지원.

### **[Speeding up V8 heap snapshots](https://v8.dev/blog/speeding-up-v8-heap-snapshots)**

- V8팀에서 문제를 인지하고, 범위를 좁히고, 정량화하고 해결하기까지의 과정 feat.Bloomberg
    - nodejs에서는 `require('v8').writeHeapSnapshot();` 를 통해 스냅샷을 찍는데 500MB에 30분이 걸리는 문제 발생
    - 블룸버그 팀에서 Windows의 성능 분석기를 사용해보니 각 노드를 방문하고 이름을 수집하는데 대부분의 시간을 소요
    - `ComputeStringHash` 에서 문제를 찾았고 해시 알고리즘 수정.
        - 최적화들을 진행 후 테스트, 100MB 10분 ⇒ 6초로 단축

### **[Publishing with npm provenance from private source repositories is no longer supported](https://github.blog/changelog/2023-07-26-publishing-with-npm-provenance-from-private-source-repositories-is-no-longer-supported/)**

- private repo는 npm provenance 와 함께 퍼블리시하지 못하도록 변경

### **[Enquirer: Stylish CLI prompts](https://github.com/enquirer/enquirer)**

- nodejs에서 cli 프롬프트 만드는 도구
- eslint, webpack, yarn, pm2, pnpm, lighthouse등에서 사용하는 도구

### **[ora: Elegant terminal spinner](https://www.notion.so/2023-08-02-a317ed7369a44645bab4b3f7f4021d1d?pvs=21)**

- 터미널 스피너 7.0 릴리즈. 노드버전 최소 16 필요.

### **[hackathon-starter 8.0](https://github.com/sahat/hackathon-starter/releases/tag/8.0.0)**

- 해커톤을 위한 nodejs 부트스트랩 앱 8.0 릴리즈

# Javascript

### **[Aniso: An Open Source ASCII Tool to Generate Text-Based Imagery](https://aniso.studiofreight.com/)**

- 문자 기반 이미지를 생성하는 오픈소스 아스키 도구
- 미디어 파일을 올리면 아스키 코드로 이루어진 3D 렌더링

### **[VanJS: World's smallest reactive UI framework](https://vanjs.org/)**

- 1.0 릴리즈 - [https://github.com/vanjs-org/van/releases/tag/1.0.0](https://github.com/vanjs-org/van/releases/tag/1.0.0)
- Pure JS, DOM을 사용한 초경량(0.9Kb), 제로 디펜던시 UI 프레임워크

### **[More Control Loading the Maps JavaScript API](https://cloud.google.com/blog/products/maps-platform/more-control-loading-maps-javascript-api?hl=en)**

- 구글 맵 라이브러리 디펜던시 로드되는 시기 제어 가능
- 성능 개선 - 정적 파일에 대해 Brotil 압축, 스크린 바깥은 지연 로딩
- `<script>` 를 사용하는 이유 - 많은 사이트들이 적극적으로 유지보수되고 있지 않음. 내부를 업데이트 해야 할 때 사용자들의 업데이트를 대신 처리.

### **[Understanding React Server Components](https://vercel.com/blog/understanding-react-server-components)**

- React Sever Component에 대한 vercel의 설명
- RSC는 클라이언트 컴포넌트를 대체하기 위한게 아니라는 점 유의

### **[Type vs Interface: Which Should You Use In 2023?](https://www.totaltypescript.com/type-vs-interface-which-should-you-use)**

- TS에서 Type과 Interface의 차이.
- type은 캐싱되지 않음으로 인한 성능 차이
- interface는 선언 병합이 되고, 객체 상속 가능. 확장 가능하기 때문에 갖고 있는 인덱스 시그니처 이슈 등

### **[size-limit](https://github.com/ai/size-limit)**

- JS앱, lib를 실행하는 비용을 비용 계산기
- ci시스템에 병합하여 github pr에 주석으로 번들 크기 변경 사항 게시 가능

# ETC

### **[Vision for W3C](https://www.w3.org/TR/2023/DNOTE-w3c-vision-20230725/)**

- W3C의 미션, 가치, 목적, 원칙을 표현하는 문서
- W3C의 비전은 더 포용적이고 사용자를 존중하는 웹. 거짓보다 진실을, 이익보다 사람을, 증오보다 인류애를 지지하는 웹을 만드는 것

### **[One-time permissions in Chrome](https://developer.chrome.com/blog/one-time-permissions/)**

- 기존의 크롬은 권한에 있어서 영구 차단, 영구 허용, 임시차단만 존재.
- 크롬 116부터는 일시적인 허용 추가.
- 일시적 허용에 대한 모범 사례, 권한 만료, 크롬에서의 UI 등에 대한 설명

### Release

- [Release Notes for Safari Technology Preview 175](https://webkit.org/blog/14398/release-notes-for-safari-technology-preview-175/)
- [Backbone 1.5](https://github.com/jashkenas/backbone/compare/1.4.1...1.5.0)
- [What's new in Svelte: August 2023 4.1 release](https://svelte.dev/blog/whats-new-in-svelte-august-2023)
- [Marked 6.0](https://github.com/markedjs/marked/releases/tag/v6.0.0) - TS로 마이그레이션