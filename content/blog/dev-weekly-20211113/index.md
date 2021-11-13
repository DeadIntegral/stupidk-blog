---
title: dev-weekly 2021-11-13
date: "2021-11-13T10:00:00.000Z"
description: "dev-weekly 2021-11-13"
tags: ["javascript", "node", "css"]
---

# CSS

### **[enterkeyhint](https://css-tricks.com/enterkeyhint)**

- 모바일 가상 키보드에서 form action key 변경하기

### **[Tasty Buttons](https://www.htmhell.dev/26-tasty-buttons)**

- 메뉴 버튼의 다양한 사례들에 대해서 어떻게 접근성을 어기고 있는지 설명
- 바람직한 메뉴 버튼은 어떻게 만들어야 하는지 예시

### **[CleanUp.pictures](https://cleanup.pictures/)**

- 드래그한 부분을 영리하게 지워주는 도구

# Node

### [sudo rm →rf / === npm install](https://ghuntley.com/sudo-rm-rf/)

- ephemeral cloud-based 개발 환경이 대안이 될 것이라는 글
- npm에서 논의중인 내용
    - https://github.com/npm/rfcs/pull/488

# Javascript

### **['Rust is the Future of JavaScript Infrastructure'](https://leerob.io/blog/rust)**

- Rust로 대체되는 JS도구

### **[Vercel Hires Rich Harris, Creator of Svelte](https://vercel.com/blog/vercel-welcomes-rich-harris-creator-of-svelte)**

- svelte 제작자 리치 해리스 vercel로 이직

### Release

- cypress 9.0 릴리즈 - [https://github.com/cypress-io/cypress/releases/tag/v9.0.0](https://github.com/cypress-io/cypress/releases/tag/v9.0.0)
- deno 1.16 릴리즈 - [https://deno.com/blog/v1.16](https://deno.com/blog/v1.16)
- react router v6 릴리즈 - [https://remix.run/blog/react-router-v6](https://remix.run/blog/react-router-v6)

### **[The Invisible JavaScript 'Backdoor'](https://certitude.consulting/blog/en/invisible-backdoor/)**

- "*HANGUL FILLER"* 라고 불리는 "ㅤ" 를 이용한 공격
- `if(environmentǃ=ENV_PROD){` 여기 사용된 문자는 !가 아니라 "*ALVEOLAR CLICK"* 문자 항상 참이 되게 되고, 이와 같은 유니코드 문자들은 다수 존재
- Bidi 유니코드 문자를 제한하면 이와같은 형태들이 풀어서 보이게 됨

### **[hashids.js: Small Library to Generate YouTube Style IDs from Numbers](https://github.com/niieani/hashids.js)**

- 유튜브 스타일의 ID 를 생성(인코드 및 디코드)해주는 라이브러리