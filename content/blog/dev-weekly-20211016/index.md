---
title: dev-weekly 2021-10-16
date: "2021-10-16T10:00:00.000Z"
description: "dev-weekly 2021-10-16"
tags: ["javascript", "node", "css"]
---

# CSS

### **[Animation Techniques for Adding and Removing Items From a Stack](https://css-tricks.com/animation-techniques-for-adding-and-removing-items-from-a-stack)**

- ontransitionend 활용
- 애니메이션의 축을 바꿔서 연속된 지오메트리 변환 줄이기

### **[Endurance Spacecraft - Interstellar - Pure CSS](https://codepen.io/josetxu/pen/gORKrgR)**

- only html, css로 만든 스페이스크래프트

# Node

### **[Retiring the Node.js Community Committee](https://nodejs.org/en/blog/announcements/retiring-the-node-js-community-committee/)**

- Nodejs 커뮤니티 위원회 은퇴, 기존 이니셔티브를 Nodejs TSC로 이동

### **[npm 8.0 Released (But It's Not a Huge Deal)](https://github.blog/changelog/2021-10-07-npm-cli-upgraded-to-version-8/)**

- require('npm') 지원 중단
- node 10, 11 지원 중단
- 12, 14의 지원을 ^12.13.0, ^14.15.0 으로 높임

# Javascript

### **[Parcel v2 Released](https://parceljs.org/blog/v2/)**

- First-class SVG support
- Image optimizer - 무손실 압축 지원
- Service worker runtime
- Gzip and Brotli compression

### **[ESLint v8.0.0 Released](https://eslint.org/blog/2021/10/eslint-v8.0.0-released)**

- ES2022 신택스 완벽 지원
- ES3에서 식별자로 예약어 사용불가

### **[How AWS Halved the Publish Size of Its AWS SDK for JavaScript Packages](https://aws.amazon.com/ko/blogs/developer/how-we-halved-the-publish-size-of-modular-aws-sdk-for-javascript-clients/)**

- AWS SDK 설치 용량 40%가량 감소
    - 트랜스파일된 `*.js` 파일에서 주석 삭제
    - downleveled `*.d.ts` 파일에서 주석 삭제
    - TS 소스코드 제거, 소스맵 파일 제거

### **[Board Gaming in Figma (with JavaScript)](https://mastery.games/post/board-gaming-in-figma/)**

- 피그마로 보드게임 만드는 과정
- 마스터 보드 컴포넌트를 만들고, 상대 페이지에 180도 회전한 인스턴스 배치
- 피그마는 HTML, CSS, JS를 지원. feat.플러그인 API

### **[Sapling: VS Code Extension for Traversing Your React Component Hierarchy](https://medium.com/@saplingextension/introducing-sapling-a-vs-code-extension-for-traversing-your-react-component-hierarchy-3ac94d95887e)**

- 파일 단위로 보여주는 것이 아니라, 참조중인 의존성 단위의 컴포너트를 보여주는 플러그인

### **[DOOM Rendered via Checkboxes](https://healeycodes.com/doom-rendered-via-checkboxes)**

- 체크박스로 만든 둠