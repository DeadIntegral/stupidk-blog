---
title: dev-weekly 2022-07-23
date: "2022-07-23T08:00:00.000Z"
description: "dev-weekly 2022-07-23"
tags: ["javascript", "node", "css"]
---


# CSS

### **[Holograms, Light-Leaks and How To Build CSS-Only Shaders](https://robbowen.digital/wrote-about/css-blend-mode-shaders)**

- `mix-blend-mode` 를 이용한 다양한 예제들 - 오로라, 빛반사, 홀로그램
- CSS shader, 이미지에 입힌 반사광, `background-attachment: fixed` 를 통한 스크롤 보정등으로 조명만들기
- mix-blend-mode 에 대한 기본적인 사용법과, 레이어 합성에 대한 개념

### **[Avoiding <img> layout shifts: aspect-ratio vs width & height attributes](https://jakearchibald.com/2022/img-aspect-ratio)**

- 이미지 레이아웃 시프트 피하기
- aspect-ratio attr같이쓰는것과 같이 잘못 알려진 부분에 대한 교정

### **[Technical Writing for Developers](https://css-tricks.com/technical-writing-for-developers)**

- 개발자를 위한 글쓰기
- 주석
    - 주석은 코드의 반복이 아니라 가치를 더해야 하고, 현재 코드를 반영해야 함
- PR 작성하기
    - 변경 사항 및 변경 이유 요약
- 버그 리포트
    - 스크린샷, 재현방법 등

### **[Min-Max-Value Interpolation](https://min-max-calculator.9elements.com/)**

- 원하는 MIN, MAX와 뷰포트의 MIN, MAX를 입력하면 clamp 를 생성해주는 도구

# Node

### **[Etro: Video-Editing Framework for Browser and Node](https://etrojs.dev/)**

- 코드로 영상편집하는 프레임워크 Etro

# Javascript

### **[Reducing the Size of a Large JavaScript SDK Package by 29%](https://blog.sentry.io/2022/07/19/javascript-sdk-package-reduced)**

- 센트리 JS SDK 번들크기 29% 감소하기까지의 과정들

### **[Using Hermes’s Quicksort to run Doom: A tale of JavaScript exploitation](https://engineering.fb.com/2022/07/20/security/hermes-quicksort-to-run-doom/)**

- 헤르메스 엔진의 퀵소트를 이용하여 Doom 실행하기
- 퀵 소트 도중 배열을 수정하며 인덱스 버퍼에 대한 OOB를 발생시키기
    - 전략적 메모리 레이아웃 생성
    - 소트 버그를 이용하여 malloc 청크 크기 변경과 오버랩핑 청크(arrayBuffer) 획득
    - 오버랩핑 버퍼 중 하나를 GC 세그먼트로 교체해서 read, wright 권한 획득하기

### **[Thoughts on Integer Math in JavaScript](https://james.darpinian.com/blog/integer-math-in-javascript)**

- `| 0` 을 붙여서 JS에서 int 연산으로 변환하기

### **[JavaScript Obfuscation Techniques by Example](https://www.trickster.dev/post/javascript-obfuscation-techniques-by-example/)**

- JS 의 다양한 난독화 기술들에 대한 소개