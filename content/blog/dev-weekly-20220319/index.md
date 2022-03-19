---
title: dev-weekly 2022-03-19
date: "2022-03-19T11:00:00.000Z"
description: "dev-weekly 2022-03-19"
tags: ["javascript", "css", "node"]
---
# CSS

### **[A Look at the Dialog Element's Super Powers](https://www.stefanjudis.com/blog/a-look-at-the-dialog-elements-super-powers)**

- `dialog` modal 은 `dialog.show()`을 하면 닫기 버튼으로 자동으로 포커스해주고,  `dialog.close()`를 하면 이전의 요소로 포커스가 이동되고, ESC로 닫히고, TAB을 눌렀을 때 다른 요소로의 접근을 막음. (접근성에 매우 강력)
- showModal로 열었을 때 배경은  `::backdrop` 으로 처리 가능
- 사파리 15.4와 파이어 폭스도 이를 지원

### **[Pure CSS - Pikachu in 3D Box](https://codepen.io/maxi83c/pen/JjOZdWX)**

- HTML, CSS만으로 만든 피카츄가 들어있는 박스. 클릭 상태를 유지하면 박스가 열리고 피카츄가 나옴

# Node

### **[peacenotwar: How an npm Package Protested Russia's Invasion of Ukraine](https://snyk.io/blog/peacenotwar-malicious-npm-node-ipc-package-vulnerability/)**

- 새 라이브러리를 만들고, vue cli에 의존성으로 포함시킴
- 해당 라이브러리를 업데이트 하면서 러시아나 벨라루스의 지리적 위치와 일치하면 모든 시스템에 대해 공격

### **[Faker 6.0: Generate Massive Amounts of Fake Data](https://github.com/faker-js/faker/releases/tag/v6.0.0)**

- 1월에 메인테이너의 이슈 이후 커뮤니티에서 faker.js 계승
- ESM 지원을 포함하는 첫 메이저 릴리즈 v6
- 계승(인수) - [https://fakerjs.dev/update.html](https://fakerjs.dev/update.html)

### **[Why and How to Use HTTPS in Your Local Development Environment](https://auth0.com/blog/using-https-in-your-development-environment/)**

- 로컬 개발 환경에서 HTTPS를 사용했을 때 장점 - Environment parity, Strong security policies, Using specific browser features, Custom hostname
- 인증서 생성하고, 노드에서 HTTPS 적용하는 과정 설명

### **[Taiko: A Library and REPL to Automate Browsers](https://github.com/getgauge/taiko)**

- nodejs 웹 어플리케이션 테스팅 라이브러리 (playwright와 유사)
- repl 모드가 존재.
    - repl 모드에서 콘솔로 웹을 서핑하고, `.code` 를 입력하면 지금까지 과정을 e2e code로 생성

# Javascript

### **[Prettier 2.6 Released](https://prettier.io/blog/2022/03/16/2.6.0.html)**

- Prettier 2.6 릴리즈 - rollup에서 esbuild로 전환, TS4.6 지원
- `singleAttributePerLine` 추가 - 한 줄에 하나의 속성만 있게하는 옵션
    - Prettier의 철학과 맞지 않아 오래 고민했지만 많은 유저들이 원해 추가한 기능

### **[Deno 1.20 Released](https://deno.com/blog/v1.20)**

- JS와 Rust의 커뮤니케이션 레이어 60% 성능 향상
- HTTP Response body 자동 압축
- deno bench 명령어 추가 - V8이 최적화 할 수 있도록 1000회의 워밍업 후, 다음1000회를 측정
- TS 4.6, V8 10.0 지원 등

### **[Next.js's New Official 'Foundations' Course](https://nextjs.org/learn/foundations/about-nextjs)**

- Nextjs 새로운 공식 기초 과정 출시

### **[Upgrading Next.js for Instant Performance Improvements](https://vercel.com/blog/upgrading-nextjs-for-instant-performance-improvements)**

- vercel팀이 VRS라는 서버리스 데모앱의 next버전을 8에서 12로 올리는 과정과 이펙트