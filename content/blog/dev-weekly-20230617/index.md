---
title: dev-weekly 2023-06-17
date: "2023-06-17T16:10:00.000Z"
description: "dev-weekly 2023-06-17"
tags: ["javascript", "css", "node", "go", "etc"]
---
# CSS

### **[Rebuilding a comment component with modern CSS](https://ishadeed.com/article/comment-component/)**

- 코멘트와 리코멘트가 연결된 복잡한 레이아웃 css로 만들기
- feat. `grid`, `subgrid`, `grid-column: 1 / -1` , 곡선 그리기 등
- [https://codepen.io/shadeed/pen/GRwKVvY/d1aa1dd4fc228c3ec5f9d2849e706ca6](https://codepen.io/shadeed/pen/GRwKVvY/d1aa1dd4fc228c3ec5f9d2849e706ca6)

### **[My Custom CSS Reset](https://www.joshwcomeau.com/css/custom-css-reset/)**

- CSS Reset은 10년정도 동안 업데이트 없기 때문에 만들어본 커스텀 reset
- 왜 그런 프로퍼티로 리셋하는지와 유용한 팁 설명
    - isolation: isolate; 를 설정하면 스택킹 컨텍스트 버그나 z-index 경쟁 없는 쌓임맥락 생성.

# Node

### **[Node v20.3.0 (Current) Released](https://nodejs.org/en/blog/release/v20.3.0)**

- 마이너 릴리즈지만 libuv 1.45.0 도입으로 리눅스에서 성능 개선
    - libuv 1.45.0 에서는 io_uring 지원. io_uring을 사용하면 8배의 성능 향상.
    - [https://blog.desdelinux.net/libuv-una-biblioteca-multiplataforma-utilizada-en-muchos-proyectos-para-el-soporte-para-e-s/](https://blog.desdelinux.net/libuv-una-biblioteca-multiplataforma-utilizada-en-muchos-proyectos-para-el-soporte-para-e-s/)

# Javascript

### **[No, ‘AI’ Will Not Fix Accessibility](https://adrianroselli.com/2023/06/no-ai-will-not-fix-accessibility.html)**

- AI는 접근성을 개선하지 못함. 해당 이미지가 생겨나는 맥락을 모르고 단편적인 정보만을 갖고 있기 때문.

### **[Melange 1.0 is here](https://buttondown.email/anmonteiro/archive/melange-hits-v10/)**

- 버클 스크립트(리스크립트)의 포크로 시작되어 OCaml과의 호환성을 유지하는 툴체인
- JS로 OCaml을 컴파일

### **[Angular v16.1.0](https://github.com/angular/angular/releases/tag/16.1.0)**

- TS 5.1 지원
- 앵귤러의 새로운 컨트롤 플로우 신택스
    - [https://github.com/angular/angular/discussions/50719](https://github.com/angular/angular/discussions/50719)

### **[Bun v0.6.9](https://bun.sh/blog/bun-v0.6.9)**

- Bun.serve() 메모리 개선
- Bun 초기 설치 메모리 50% 감소
- 런타임에서 모듈 임포트 메모리 사용량 감소
- CommonJS Require 충돌 수정

### **Release**

- [ts-pattern 5.0](https://github.com/gvergnaud/ts-pattern/releases/tag/v5.0.0)
- [nest 10.0](https://github.com/nestjs/nest/releases/tag/v10.0.0)

# ETC

### **[Video-based Cryptanalysis: Exploiting a Video Camera's Rolling Shutter to Recover Secret Keys from Devices Using Video Footage of Their Power LED](https://www.nassiben.com/video-based-crypta)**

- LED 비디오 영상을 사용하여 손상되지 않은 장치에서 비밀 키 복구
- 장치의 CPU 가 수행하는 암호화 계산이 장치 전원 LED 밝기에 영향을 미치는 전력 소비를 변경.
    - 16미터 떨어진 곳에 있는 하이재킹된 인터넷 연결 보안 카메라를 통해 스마트 카드의 256bit ECDSA(타원 곡선 디지털 서명)키 복구
    - iPhone13 Pro Max 를 통해 로지텍 스피커의 전원 LED를 분석하여 S8의 378bit SIKE 키 복구

### **[Chrome for Testing: reliable downloads for browser automation](https://developer.chrome.com/blog/chrome-for-testing/)**

- 일반 사용자는 크롬의 자동업데이트가 목적에 잘 부합하지만, 특정 버전에서 재현해봐야 하는 엔지니어들은 고통.
- 이에 대해 엔지니어들이 크로미움 프로젝트의 특정 버전을 설치해서 테스팅하는 것을 알고있고, 새로운 대안으로 버전 지정이 가능한 테스트용 바이너리 크롬 공개

### **[The Stack Overflow Developer Survey 2023 Results](https://survey.stackoverflow.co/2023/)**

- 약 9만명 설문참여. AI 항목 추가.

### **[VSCode **May 2023 (version 1.79)**](https://code.visualstudio.com/updates/v1_79)**

- TS 5.1.3 지원, 곧 릴리즈할 TS 5.2 지원.
- `"editor.linkedEditing": true` 으로 JSX 닫기 태그 동시 수정 지원
- JSDoc `@Pramas` 자동완성에서 누락된 모든 매개변수 제안 표시
- Window 8, 8.1 지원 종료