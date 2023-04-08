---
title: dev-weekly 2021-04-10
date: "2021-04-10T09:40:00.000Z"
description: "dev-weekly 2021-04-10"
tags: ["javascript", "css", "go", "db"]
---

# CSS, Go, Node

## CSS

[React-Menu](https://github.com/szhsin/react-menu)

- 드랍다운, 서브메뉴, 컨텍스트 메뉴 등이 존재하는 리액트 컴포넌트
- 사용자 정의가 가능하고, 키보드 인터랙션 존재
- WAI-ARIA 준수

---

## GO

### **[PTerm: A Modern Go Module to Beautify Console Output](https://github.com/pterm/pterm/)**

- go beauty module
- 크로스 플랫폼(윈도, 맥, 리눅스 100% 호환)
- 콘솔에 차트, 큰글자, 박스, 트리 등 다양한 기능 제공

### **TiDB 5.0: A Distributed HTAP Database**

- TiDB 5.0 릴리즈
- Go로 작성된 수평확장성을 제공하는 디비
- MySQL의 프로토콜과 호환되는 오픈 소스 분산 HTAP 데이터베이스
    - Hybrid Transactional and Analytical Processing

---

## Node

### **[Node Development with Docker and Docker Compose](https://www.nodejsdesignpatterns.com/blog/node-js-development-with-docker-and-docker-compose/)**

- docker container란 무엇인지, 왜 도커를 사용해야 하는지 설명
- node를 docker, docker-compose로 구성하는 방법과 장단점

## [PM2 WebUI: An Open-Source Alternative to PM2 Plus](https://github.com/suryamodulus/pm2-webui)

- pm2 웹버전

---

# Javascript

### **[The ES2021 Edition “JavaScript for Impatient Programmers”](https://gist.github.com/rauschma/e9c00fddc17e73fab6ce6c22b2e78e17)**

- JavaScript for Impatient Programmers의 저자 Dr. Axel가 내용을 ES2021로 업데이트
- 책의 상당수는 [https://exploringjs.com/impatient-js/](https://exploringjs.com/impatient-js/) 여기서 무료로 보기 가능

## Quick Bits

### **[https://developer.chrome.com/blog/migrating-to-typescript/](https://developer.chrome.com/blog/migrating-to-typescript/)**

- 구글 데브툴즈팀이 클로저 컴파일러에서 TS로 마이그레이션했대영
ts도입까지의 과정, 마이그레이션과정, 마이그레이션 후 영향 등이 있어여
<del>ts로 바꾸고 빌드 타임이 늘어났다네여</del>

## Code & Tools

### **[CSS-Select 4.0: A CSS Selector Compiler and Engine](https://github.com/fb55/css-select)**

- css selector 4.0 릴리즈
- 기존의 css selector는 left to right 라서, css처럼 상향식 파서를 구현해 성능 향상

### **[moovie.js: A Movie-Focused HTML5 Media Player](https://github.com/BMSVieira/moovie.js)**

- 커스텀 가능하고, 의존성 없고, 반응형이고 단축키 지원하는 무비 플레이어
- .vtt, .srt 캡션 파일 지원 하고 로컬의 파일을 플레이어에 업로드 가능