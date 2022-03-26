---
title: dev-weekly 2022-03-26
date: "2022-03-26T14:00:00.000Z"
description: "dev-weekly 2022-03-26"
tags: ["javascript", "css", "node"]
---
# CSS

### **[Building a Loading Bar Component](https://web.dev/building-a-loading-bar-component)**

- Loading bar 만들기 - progress element
    - 접근성을 고려한 마크업
    - 다크 테마를 고려한 스타일링, 크로스 브라우징
    - 애니메이션
    - JS를 통한 실제 값과 바인드

### **['color-scheme' CSS 속성과 해당 메타 태그를 사용하여 다크 모드 기본 스타일을 개선](https://web.dev/color-scheme/)**

- UA style sheet에 대한 설명
- color-scheme 와 prefers-color-scheme 같이 사용하기

### **[CSS Blossoming Flowers at Magical Night](https://codepen.io/mdusmanansari/pen/BamepLe)**

- Pure CSS - 꽃 애니메이션

# Node

### **[Tao of Node: On Design, Architecture and Best Practices](https://alexkondov.com/tao-of-node/)**

- 유사한 구조의 Node 앱을 찾기 어렵고, 이는 다른 언어를 공부하던 사람 입장에서 집인장벽. 노드 앱을 구축하기 위해 확립한 원칙들(전부 의견)

### **[Malicious npm Packages Targeting Azure Developers](https://jfrog.com/blog/large-scale-npm-attack-targets-azure-developers-with-malicious-packages/)**

- typosquatting을 이용한 공격방식
    - ex) @azure/core-tracing ⇒ core-tracing 패키지 스코핑을 제외한 라이브러리를 만들고 악성코드 삽입

### **[Dum: An `npm` Script Runner Written in Rust](https://github.com/egoist/dum)**

- Rust로 작성된 npm script runner - 보다 빠른 성능이 목적

### **[Chrome Extension CLI: CLI for Building Chrome Extensions](https://github.com/dutiyesh/chrome-extension-cli)**

- 빠르게 크롬 확장 프로그램을 만들 수 있도록 돕는 도구

# Javascript

### **[Parcel v2.4.0 Released: The Zero Config Build Tool](https://parceljs.org/blog/v2-4-0/)**

- Parcel 2.4.0 릴리즈
- Parcel CSS
    - Cascade layers, 커스텀 프로퍼티
    - lab()를 포함한 CSS Color level4, 레거시 브라우저에대한 fallback

### **[RFC: Intent to Ship React 18](https://github.com/reactjs/rfcs/blob/react-18/text/0000-react-18.md)**

- React 18의 새로운 기능과 변경을 다루는 RFC

### [AWS Lambda now supports up to 10GB of ephemeral storage](https://aws.amazon.com/ko/blogs/aws/aws-lambda-now-supports-up-to-10-gb-ephemeral-storage/)

- AWS 람다가 이전 512MB 제한에서 최대 10GB 제한으로 변경 (선택 가능)
    - 과거 미디어 트랜스 코딩과 같은 작업을 할 때 큰 데이터는 로컬 캐싱을 못해서 개발자를 힘들게 함

### **[An Introduction to AWS CloudFront Functions](https://www.honeybadger.io/blog/aws-cloudfront-functions/)**

- AWS CloudFront Function 소개
- AWS 엣지 로케이션에 배포하기 - 람다 엣지와의 차이점

### **[Ladle: Develop and Test Your React Stories Faster](https://www.ladle.dev/blog/introducing-ladle/)**

- Vite 기반의 ESM을 통해 성능 향상
- 번들 사이즈 개선 및 코드 스플리팅
- 스토리북 대체가 목표