---
title: dev-weekly 2021-10-09
date: "2021-10-09T21:30:00.000Z"
description: "dev-weekly 2021-10-09"
tags: ["javascript", "node", "css"]
---

# CSS

### [Conditional Border Radius In CSS](https://ishadeed.com/article/conditional-border-radius)

- 미디어 쿼리를 사용하지 않고, 조건에 따른 radius 만들기
    - `border-radius: max(0px, min(8px, calc((100vw - 4px - 100%) * 9999)));`
- `clamp` 는 사파리12에서 지원하지 않음

### [Take the State of CSS 2021 Survey](https://stateofcss.com/)

- CSS State Survey

### [Understanding Logical Focus Order](https://devyarns.com/logical-focus-order)

- display none이나 visibility hidden으로 요소를 숨겨도 포커스가 이동될 수 있음
    - `tabindex="-1"`도 주면 이동되지 않게 가능
- 가능한 tabindex는 사용하지 않는게 좋음

### [Sci-Fi Art: A Vacuum From Space](https://codepen.io/ivorjetski/pen/ZEyyzXm)

- CSS로 그린 그림. 매우 많이 버벅임

# Node

### [Writing Clean JavaScript Tests with the BASIC Principles](https://yonigoldberg.medium.com/fighting-javascript-tests-complexity-with-the-basic-principles-87b7622eac9a)

- 테스팅을 포기하는 이유
    - 테스팅에 if, for 등 로직이 들어가면 안됨
- 우리는 어떻게 테스팅을 할 수 있을지
- BASIC 원칙

### [Announcing TypeScript 4.5 Beta](https://devblogs.microsoft.com/typescript/announcing-typescript-4-5-beta/)

- Node에 대한 ES 모듈 지원

### [emoji-regex: A Regular Expression to Match All Emoji-Only Symbols](https://github.com/mathiasbynens/emoji-regex)

- 유니코드 표준과 일치하는 이모지 정규식 제공

# Javascript

### [How Kent C Dodds Built a Modern Website in 2021](https://kentcdodds.com/blog/how-i-built-a-modern-website-in-2021)

- pipeline, flow 등 그림을 통한 설명
- MSW 로 데이터 모킹
- Cloudinary를 통한 이미지 최적화 - 가격이 좀 비쌈
- Prisma와 DB 인터랙션

### [jQuery Maintainers Continue Modernization Initiative; Deprecate jQuery Mobile](https://blog.jquery.com/2021/10/07/jquery-maintainers-continue-modernization-initiative-with-deprecation-of-jquery-mobile/)

- JQuery Mobile 디프리케이트
- JQuery UI 는 maintenance only mode로 변경

### [new VS Code release](https://code.visualstudio.com/updates/v1_61)

- VSCode 1.61 - TS4.5 지원

### [13 terrific entries to the js13kGames competition](https://github.blog/2021-10-05-13-tiny-and-terrific-entries-from-the-js13kgames-competition/)

- 13kb로 게임만들기 대회 출품작들의 짧은 비디오 클립
- 올해의 주제는 Space

### [Safe DOM Manipulation (in the Future) with the Sanitizer API](https://web.dev/sanitizer/)

- innerHTML과 같이 직접 돔 조작을 하지만, 안전하게 조작하는 API
- 크롬과 파이어폭스에서는 flag를 활성화해서 이용 가능

### [Getting Started with the Rollup.js JS Bundler](https://blog.openreplay.com/the-ultimate-guide-to-getting-started-with-the-rollup-js-javascript-bundler)

- 롤업 시작하기

### [A Guide to CSS Debugging](https://www.smashingmagazine.com/2021/10/guide-debugging-css/)

- 특정 엘리먼트 - 우클릭 - 스타일 복사 ⇒ CodeSandBox등에 붙여넣어보기
- 오버플로
    
    ```css
    * {
    	outline: 1px solid red;
    } // border가 아니라 outline인 이유는 dom크기 및 기존 border에 영향을 주지 않아서
    ```
    
    - FF를 사용하면 DOM에 오버플로 되는 요소 표시
- [https://piccalil.li/blog/a-modern-css-reset/](https://piccalil.li/blog/a-modern-css-reset/)

### [Xterm.js: A Terminal/Shell Component for the Front End](https://xtermjs.org/)

- 웹용 터미널
- VSCode, cPanel, Azure Cloud Shell 등 많은 프로젝트에서 사용

### [Immutable JS 4.0: Immutable Persistent Data Collections](https://github.com/immutable-js/immutable-js/releases/tag/v4.0.0)