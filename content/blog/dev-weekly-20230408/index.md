---
title: dev-weekly 2023-04-08
date: "2023-04-08T014:40:00.000Z"
description: "dev-weekly 2023-04-08"
tags: ["javascript", "css"]
---
# CSS

### **[CSS Masking](https://ishadeed.com/article/css-masking/)**

- CSS Mask가 interop 2023에 포함되어 브라우저 지원 기대
- 마스킹은 요소의 일부를 지우지 않고 숨기는 방식으로 작동
- 마스크의 작동 방식, 예제, 실제 사용 사례 소개

### **[CSS Creator Håkon Wium Lie Interview](https://evrone.com/hakon-wium-lie-interview)**

- CSS 창시자 겸 1998~2016년 오페라 CTO로 활동한 Hakon Wium Lie 인터뷰
- 어떻게 CSS를 만들게 되었는지, HTML+CSS를 사용하여 수동으로 웹사이트 구축하는것, 웹의 미래, 메타버스, chatGPT 등 에 대한 질의응답

# Javascript

### **[RFC: Angular Signals](https://github.com/angular/angular/discussions/49685)**

- 앵귤러 시그널의 목표, 구성 QnA
- 4가지 하위 문서 - 시그널의 선택 이유에 대한 RFC, 시그널 API 에 대한 RFC, 시그널 기반 컴포넌트 RFC, RxJS와의 상호운용 RFC
- 오늘날 앵귤러 변경 감지가 작동하는 방식에 대한 설명(zone.js 와 top down 변경 감지)

### **[Framework popularity on Netlify](https://www.netlify.com/blog/framework-popularity-on-netlify/)**

- Netlify 에서 가장 많이 사용되는 라이브러리
- 설문 조사에서는 개발자의 71%가 리액트 사용

### **[Pausing Manifest V2 phase-out changes](https://groups.google.com/a/chromium.org/g/chromium-extensions/c/zQ77HkGmK9E/m/HjaaCIG-BQAJ)**

- Manifest V3 마이그레이션 계획 공유. 2024년에 MV2 종료를 위한 실험 예정이고 최소 6개월의 마이그레이션 시간 제공할 것.
- [https://developer.chrome.com/docs/extensions/migrating/to-service-workers/](https://developer.chrome.com/docs/extensions/migrating/to-service-workers/)
    - 백그라운드 스크립트와 SW의 차이점. 마이그레이션 시 차이점.

### **[WebAssembly tail calls](https://v8.dev/blog/wasm-tail-call)**

- V8 에서 WASM에 대한 tail call 제공
    - emscripten은 -mtail-call 라는 옵션 제공
- tail call 은 엔진의 책임이 아닌 tool chain의 업스트림으로 수행되어야 할 일. TurboFan에서 할 일은 호출 종류와 대항 함수 시그니처에 따라 적절한 시퀀스 인스트럭션을 생성하는 것.

### **[Chrome ships WebGPU](https://developer.chrome.com/blog/webgpu-release/)**

- Chrome 113 부터 WebGPU 제공. FF, Safari도 지원 진행중
- W3C WebGPU 그룹의 공동 노력 결과. 2017년부터 6년간의 개발.
- WebGL이 제공 안하는 고급 기능 접근 가능
- Babylon.js, PlayCanvas, Tensorflow.js, Three.js 등은 구현중이거나 이미 지원 (한줄 변경하면 지원)

### Release

- [Electron 24.0](https://www.electronjs.org/blog/electron-24-0)
- [Storybook 7.0](https://github.com/storybookjs/storybook/releases/tag/v7.0.0)
- [React-chrono 2.0](https://github.com/prabhuignoto/react-chrono/releases/tag/2.0) - 글 작성 시점에 2.1 릴리즈
- [Framework7 8.0](https://github.com/framework7io/framework7/releases/tag/v8.0.0)
- [eruda 3.0](https://github.com/liriliri/eruda/releases/tag/v3.0.0)

### **[Getting PWAs in App Stores with PWABuilder](https://web.dev/pwas-in-app-stores/)**

- 다양한 앱 스토어에 제출할 패키지를 만들어주는 도구 PWABuilder
- 전제조건 및 패키지 게시까지의 간략한 과정 소개
- [https://www.pwabuilder.com/](https://www.pwabuilder.com/)

### **[Are Safari Releases Causing 'Development Hell'?](https://www.construct.net/en/blogs/ashleys-blog-2/safari-releases-development-1616)**

- 사파리 릴리즈로 인해 발생했던 일들에 대한 전말과 입장 표명
    - Construct 프로젝트는 zip 파일 기반으로 하며 zip.js를 사용. 지원되는 경우 Compression Streams API 를 사용하는데 사파리 16.4의 api는 zip.js와 호환 불가. 버그를 보고했고 수정한다고 했지만 STP에서 여전히 버그가 발생했고, 릴리즈 때 수정되는지 문의했지만 알려주지 않음.
    - Construct 프로젝트는 OffscreenCanvas를 사용하는데 애플은 이를 지원하지만 2d는 지원하지 않음. `typeof OffscreenCanvas !== "undefined"` 에서 문제가 발생.
- 애플이 이미 알고 있지만 알려주지 않는 것들로 인한 문제