---
title: dev-weekly 2023-10-07
date: "2023-10-07T10:40:00.000Z"
description: "dev-weekly 2023-10-07"
tags: ["javascript", "node", "browser"]
---
# Node

### **[Honey, I shrunk the npm package](https://jamiemagee.co.uk/blog/honey-i-shrunk-the-npm-package/)**

- npm 패키지는 기본적으로 `tar.gz`, `tgz` 로 제공.
- npm의 압축 전략 현대화 가능성을 위해 Brotli, zstd 를 포함하여 벤치마크
- 압축비율은 brotli, 압축 해제 시간은 zstd 가 좋음
- js구현 부족 문제, 이전 버전과의 호환성 문제

### **[Best Practices for Securing Node.js Applications in Production](https://semaphoreci.com/blog/securing-nodejs)**

- Security HTTP Header 설정, rate limit, 모니터링, https 전용 정책 채택 등 nodejs 앱을 보호하기 위한 15가지 모범 사례

# Javascript

### **[From WebGL to WebGPU](https://developer.chrome.com/blog/from-webgl-to-webgpu/)**

- WebGL과 WebGPU의 차이점.
    - WebGL은 global state가 다수 존재. 이것들은 모든 렌더링 작업에 적용되어 오류의 주된 원인이 됨. WebGPU는 상태 비저장 API 이며 전역 상태 유지하지 않음.
    - WebGPU는 CPU 버블을 피하기 위해 비동기식으로 설계.
    - 컴퓨팅 셰이더 지원 (기계학습, 물리 시뮬레이션, 사이언스 컴퓨팅 등)
    - 기존에는 GPU 메모리에서 CPU 메모리로 데이터를 복사하는 비용, 워커 및 CPU 스레드로 달성할 수 있는 병렬 처리 제한이 있었는데, WebGPU는 제한 없음
    - 캔버스 수 제한 없음. 이해하기 쉬운 오류 메시지 등

### **[Photoshop is now on the web!](https://medium.com/@addyosmani/photoshop-is-now-on-the-web-38d70954365a)**

- 어도비와 구글이 협력하여 포토샵 웹 버전 개발
- WASM(Emscripten), WebComponent(Lit), Service Worker(Workbox)
- 대용량 PSD 파일 처리를 위하여 OPFS(Origin Private File System) 제공
- 기존 포토샵의 C/Cpp 코드베이스를 WebAssembly 모듈로 포팅
    - 이미지 타일 처리와 같은 병렬 실행에서 워커 스레드 사용. SIMD, 스트리밍 인스턴스화
- 웹 컴포넌트(Lit 기반)를 통한 UI 유연성 확보
- 서비스 워커(workbox)를 사용하여 에셋, 코드 캐싱
- Tensorflow.js 를 온디바이스에서 실행하여, 클라우드가 아닌 기기에서 실행하면 성능 향상. feat.WebGPU
- 어도비는 앞으로 Creative Cloud 제품군 전체를 웹에 구축할 것.
- [https://photoshop.adobe.com/discover](https://photoshop.adobe.com/discover)

### **[An Interactive Intro to CRDTs](https://jakelazaroff.com/words/an-interactive-intro-to-crdts/)**

- CRDT(충돌 없는 복제 데이터 유형)이란 무엇인가 - 상태 기반 CRDT에 대하여
    - 상태 기반 CRDT, 작업 기반 CRDT.
    - Commutativity, Associativity, Idempotence 보장이 필요
- LWW(Last Write Wins) Register
    - 수신된 타임스탬프와 로컬 타임스탬프를 기반으로 마지막으로 발생한 쓰기로 결정.
- LWW(Last Write Wins) Map 의 작동 방식

### **Release**

- [Critical 6.0](https://github.com/addyosmani/critical/releases/tag/v6.0.0) - 렌더링 되는 영역의 css를 인라인으로 처리해서 성능향상 시키는 노드 도구
- [Astro 3.2](https://astro.build/blog/astro-320/) - view transition 개선
- [redux-toolkit 1.9.7](https://github.com/reduxjs/redux-toolkit/releases/tag/v1.9.7)
- [CKEditor5 40.0](https://github.com/ckeditor/ckeditor5/releases/tag/v40.0.0)

# ETC

### **[Get ready for Interop 2024](https://webkit.org/blog/14633/get-ready-for-interop-2024/)**

- 웹 표준과 인터롭 프로젝트에 대한 소개.
    - 애플, 구글, MS, 모질라 등이 웹 개발자에게 최우선 순위인 특정 기술의 상호 운용성을 지키기 위핸 노력.
- 2024 인터롭은 10월7일까지 누구나 제안서 제출 가능.
- [제안목록 링크](https://github.com/web-platform-tests/interop/issues?q=is%3Aissue+is%3Aopen+label%3Afocus-area-proposal)

### **[The Ultimate Low-Quality Image Placeholder Technique](https://csswizardry.com/2023/09/the-ultimate-lqip-lcp-technique/)**

- 저품질 이미지를 사용하더라도 LCP에 영향 없음. 해결해야 하는 두 가지 이슈
- 업스케일링 페널티. 업스케일링 해도 가장 큰 이미지로 LCP 계산
- 0.05BPP(픽셀 당 비트 수)를 지켜야 LCP요소로 간주.
    - 용량이 픽셀 수 * 0.05 / 8000 보다 커야함. ex) 1024 * 768 * 0.05 / 8000 ⇒ 약5kb

### **[Mozilla AI Guide](https://ai-guide.future.mozilla.org/)**

- 개발자가 제너레이티브 AI와 오픈소스 개발을 위한 사고방식, 개념, 실용적인 기술을 배울 수 있는 새로운 리소스

### **[Chrome now shows each active tab’s memory usage!](https://medium.com/@addyosmani/chrome-now-shows-each-active-tabs-memory-usage-4f74876538e6)**

- 크롬 탭에 마우스를 hover 하면 탭이 사용중인 메모리 표시
- 크롬 DevTools를 이용한 메모리 사용량 측정과 Perofrmance API를 통한 측정. 메모리 누수의 일반적인 원인

### **News**

- [비발디 브라우저 iOS 버전 출시. 결국 웹킷 사용](https://www.theregister.com/2023/09/28/vivaldi_browser_ios/)
- [w3c 의 새 CEO Seth Dobbs](https://www.w3.org/news/2023/w3c-announces-seth-dobbs-as-ceo/)