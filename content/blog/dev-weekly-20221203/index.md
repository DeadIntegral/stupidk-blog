---
title: dev-weekly 2022-12-03
date: "2022-12-03T19:30:00.000Z"
description: "dev-weekly 2022-12-03"
tags: ["javascript", "css", "node"]
---
# CSS

### **[Setting up a screen reader testing environment on your computer](https://www.sarasoueidan.com/blog/testing-environment-setup)**

- 스크린 리더 테스팅을 위한 환경 구성하기 (Windows Narrator, mac VoiceOver)
- 무료~프리미엄 도구들 셋팅방법 및 가이드문서들
- cheatsheet와 권장 문서들

### **[Debugging Tactics](https://addyosmani.com/blog/debugging-tactics)**

- 디버깅 할 때 첫 단계는 작동 방식에 대해 생각하는 것이 사실이 아닐 수 있다는것을 인정하는 것
- 산책하기, 오리에게 설명하기, 오류 메시지 읽기, 문서 읽기, 같은 코드를 다시 실행, 로깅
    - 내 프로젝트에 적합한 프로세스 사용하기, 문제 정의하기

### **[CSS Timeline](https://css-timeline.vercel.app/)**

- CSS 및 연관 도구들의 역사를 보여주는 타임라인

# Node

### **[EventEmitter3 5.0: A High Performance Event Emitter](https://github.com/primus/eventemitter3)**

- 브라우저와 노드를 지원하는 고성능 Event Emitter
- Nodejs의 emitter와 호환되지만 몇가지 차이점 존재
- EcmaScript3로 작성해서 컴팻이 좋음

# Javascript

### **[Speeding Up the JS Ecosystem, One Library at a Time](https://marvinh.dev/blog/speeding-up-javascript-ecosystem/)**

- 최근 Go, Rust로 도구가 다시 만들어지지만 JS는 여러 도구의 집합체. 각 도구들을 개선한 리뷰
- PostCSS - 주석이 있는지 확인하는 정규식(4.63s 중 4.6s 감소)
- SVGO
    - SVG파일의 숫자 압축에서 캐스팅이 많이 사용되어 숫자로 표현하도록 변경. (3.1s 중 1.4s 감소)
    - 소수점 처리에 있어서 문자열로 변환하고 정규식 사용하는 부분 개선. (1.7s 중 0.9s 감소)

### **[Electron 22.0 Released, Plus Other Electron News](https://www.electronjs.org/blog/electron-22-0)**

- 크롬 108, V8 10.8, Node 16.17.1 업데이트
- Windows 7/8/8.1을 지원하는 마지막 메이저 버전
- **[Introducing Electron Forge 6](https://www.electronjs.org/blog/forge-v6-release)**

### **[NextJS, SvelteKit, Remix and the future of Storybook](https://storybook.js.org/blog/framework-api/)**

- Framework - 스토리북 자동 구성 패키지
- 애플리케이션의 설정을 읽고 스토리북 자동 구축.
- Vite, NextJS, SvelteKit 지원 중, Remix, Nuxt 고려 중

### **[Tesseract.js 4.0: Pure JS OCR for Over 100 Languages](https://github.com/naptha/tesseract.js/releases/tag/v4.0.0)**

- 몇가지 브레이킹 체인지(createWorker async, getPdf replace by pdf)
- 테서랙트에서 생성한 이미지 검색, 이미지 회전 옵션 추가 등

### **[Splitting Strings into Sentences, Words or Graphemes with `Intl.Segmenter`](https://www.stefanjudis.com/today-i-learned/how-to-split-javascript-strings-with-intl-segmenter/)**

- 문자열에서 의미있는 항목(자소, 단어, 문장) 세그먼트로 분할
- 배열이 아니라 iterable로 반환하기 때문에 변환 필요
- 파이어폭스는 아직 미지원. 노드는 16부터 지원

### **[Working with Zustand for Easier React State Management](https://tkdodo.eu/blog/working-with-zustand)**

- Zustand 사용 팁

### **[V8: Pointer Compression in Oilpan](https://v8.dev/blog/oilpan-pointer-compression)**

- Tracing GC 인 Oilpan 라이브러리도 포인터 압축 지원

### **[Neutralino.js 4.9: Lightweight Cross Platform Desktop App Framework](https://github.com/neutralinojs/neutralinojs/releases/tag/v4.9.0)**

- 모든 언어의 사용자 정의 백엔드 코드를 지원하는 extensions API 제공
    - 통신을 위해 shared Websocket을 사용하기 때문에 Cpp 참조 직접 처리 불가
    - 개발자는 익스텐션 바이너리 패키징을 담당
    - 웹소켓 기반 IPC이기 때문에 네이티브 Cpp만큼 빠르지 않음

### **Release**

**[OCLIF 3.3](https://github.com/oclif/oclif)** - 세일즈포스의 nodejs cli 만드는 도구

**[Prisma 4.7](https://github.com/prisma/prisma/releases/tag/4.7.0)** - nodejs, ts를 위한 차세대 ORM

**[jsdoc-to-markdown 8.0](https://github.com/jsdoc2md/jsdoc-to-markdown)** - jsdoc 어노테이션에서 마크다운 문서 생성하는 도구