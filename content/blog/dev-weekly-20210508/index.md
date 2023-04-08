---
title: dev-weekly 2021-05-08
date: "2021-05-08T11:30:00.000Z"
description: "dev-weekly 2021-05-08"
tags: ["javascript", "css", "node"]
---
# Node, CSS

## Node

### **[V8 v9.1](https://v8.dev/blog/v8-release-91)**

- top level await 디폴트

### **[VS Code April 2021](https://code.visualstudio.com/updates/v1_56)**

- vscode 4월 릴리즈

### **[Dotenv 9.0: Load Environment Variables From .env in Node](https://github.com/motdotla/dotenv)**

- dotenv 9.0 릴리즈

### **[MapSCII: A Text-Based World Map Renderer for the Console](https://github.com/rastapasta/mapscii)**

- 소개영상 [https://asciinema.org/a/117813?autoplay=1](https://asciinema.org/a/117813?autoplay=1)
- 콘솔용 ASCII 세계지도 콘솔 렌더러. 스크롤도 작동.
- telnet [mapscii.me](http://mapscii.me) 로 접속 가능

---

## CSS

### **[A Complete Guide to Custom Properties](https://css-tricks.com/a-complete-guide-to-custom-properties)**

- CSS Variable을 overwrite하여 재활용하며 사용하는 예제

```css
button {
  --spread: 5px;
  box-shadow: 0 0 20px var(--spread) black;
}
button:hover {
  --spread: 10px;
}
```

### **[Identify and Extract Pseudo-Element Selectors From Built-In HTML Elements Using DevTools](https://www.bram.us/2021/04/15/identify-and-extract-pseudo-element-selectors-from-built-in-html-elements-using-devtools)**

- <input type="file" />, <audio> 와 같은 빌트인 엘리먼트의 스타일 지정하기
- Chrome Devtools - settings - Elements - `Show user agent showdow dom`

---

# Javascript

### **[How GitHub Uses and Works with Web Components](https://github.blog/2021-05-04-how-we-use-web-components-at-github/)**

- 깃헙은 JQuery 에서 WebComponent로 마이그레이션
- ViewComponent + Catalyst

### **[Bootstrap 5 Released](https://blog.getbootstrap.com/2021/05/05/bootstrap-5/)**

- RTL 지원
- JQuery 제거

### **Quick Bits**

- 올인원 툴 Rome 회사 설립
    - [https://rome.tools/blog/announcing-rome-tools-inc/](https://rome.tools/blog/announcing-rome-tools-inc/)
- RxJS 7.0 이 이전과 달라진 점
    - [https://medium.com/volosoft/whats-new-in-rxjs-7-a11cc564c6c0](https://medium.com/volosoft/whats-new-in-rxjs-7-a11cc564c6c0)

### **[Hosting SQLite Databases on GitHub Pages (or Any Static File Host)](https://phiresky.github.io/blog/2021/hosting-sqlite-databases-on-github-pages/)**

- 정적 호스팅 페이지에 sql.js를 사용해 디비를 구축하고, 다른 서비스가 이를 쿼리로 요처알 수 있게하는 포스트

### **[Mantine: A New React Component Library](https://mantine.dev/)**

- hook으로 작성된 리액트 컴포넌트 라이브러리
- preact에서도 작동