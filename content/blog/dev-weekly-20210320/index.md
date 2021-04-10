---
title: dev-weekly 2021-03-20
date: "2021-03-20T09:10:00.000Z"
description: "dev-weekly 2021-03-20"
tags: ["javascript", "css", "go", "db"]
---

# CSS, DB, GO, Etc

## CSS

### [Debugging Layout Shifts](https://web.dev/debugging-layout-shifts/)

- 레이아웃 시프트 디버깅하기
- 코드 스니펫 및 개발자도구 - 퍼포먼스 탭 사용법

```jsx
new PerformanceObserver((entryList) => {
  for (const entry of entryList.getEntries()) {
    if (!entry.hadRecentInput) {
      cls += entry.value;
      // debugger;
      console.log('Current CLS value:', cls, entry);
    }
  }
}).observe({type: 'layout-shift', buffered: true});
```

### [Digging Into CSS Logical Properties](https://ishadeed.com/article/css-logical-properties/)

- 다국어 지원 중 RTL 의 번거로운 작업을 대체할 프로퍼티들 소개
- margin-inline-[start, end], padding-inline-[start, end], inset-inline-[start, end] 등

### [CSS Auditing Tools](https://www.smashingmagazine.com/2021/03/css-auditing-tools/)

- [https://cssstats.com/](https://cssstats.com/)
- [https://yellowlab.tools/](https://yellowlab.tools/)
- [https://isellsoap.github.io/specificity-visualizer/](https://isellsoap.github.io/specificity-visualizer/)
- [https://www.projectwallace.com/](https://www.projectwallace.com/) 기록을 유지해주고, 웹훅을 이용하여 CI 연동 가능

## DB

### [Introducing Amazon S3 Object Lambda: Process Data During Retrieval](https://aws.amazon.com/ko/blogs/aws/introducing-amazon-s3-object-lambda-use-your-code-to-process-data-as-it-is-being-retrieved-from-s3/)

- S3의 15주년을 맞아 새로운 기능 추가

## GO

### [REST Servers in Go: Middleware](https://eli.thegreenplace.net/2021/rest-servers-in-go-part-5-middleware/)

- GO 에서 REST 서버를 작성하는 방법 시리즈 5번째 - 미들웨어

# Javascript

### [V8 Release v9.0](https://v8.dev/blog/v8-release-90)

- RegExp에서 일치하는 인덱스에 접근가능

    ```jsx
    const re = /(a)(b)/d; // d플래그
    const m = re.exec('ab');
    console.log(m.indices[0]); // 전체 매치
    console.log(m.indices[1]); // 첫 번째 캡쳐 그룹
    console.log(m.indices[2]); // 두 번째 캡쳐 그룹
    ```

- super 프로퍼티 접근속도 개선
- `for ( async of` disallowed
- JS to WASM 호출 속도 개선

## Quick Bits

[https://blog.tailwindcss.com/just-in-time-the-next-generation-of-tailwind-css](https://blog.tailwindcss.com/just-in-time-the-next-generation-of-tailwind-css)

- tailwind JIT 컴파일러

[https://github.com/nasa/openmct](https://github.com/nasa/openmct)

- 나사의 웹 기반 미션 컨트롤 프레임웤
- [https://openmct-demo.herokuapp.com/](https://openmct-demo.herokuapp.com/) 데모페이지

[https://storybook.js.org/blog/storybook-for-svelte/](https://storybook.js.org/blog/storybook-for-svelte/)

- 스벨트용 스토리북 재작성 및 DX의 모든 측면 개선
    - Zero-config setup w/ built-in TypeScript support
    - A Svelte-native story format for capturing component states
    - Auto-generated controls and documentation
    - Updated tutorials and documentation

## Articles, Opinion & Tutorials

### [Object Plus Array Is Not Zero](https://evinsellin.medium.com/object-plus-array-is-not-zero-ec4db710e7a5)

- 크롬과 AST explorer을 이용해서 일반적인 js 오해( {} + [], [] + {} )에 대해 설명
- ({} + []) 로 묶어보면 [object object]
- {}는 본래 block statement이기 때문. 크롬 콘솔창이 식으로 평가해준것
- eval에 코드를 넣어봄으로써 빠르게 확인 가능

## Code & Tools

### [React95 3.7: Windows 95-Style UI Components for React](https://github.com/arturbien/React95)

- 윈도95 스타일의 리액트 UI 컴포넌트 모음

### [Lite YouTube Embed: A Faster Youtube Embed](https://github.com/paulirish/lite-youtube-embed)

- 공식지원보다 빠른 유튜브 삽입하는 도구

### [sql.js 1.5: A Library to Run SQLite on the Web](https://github.com/sql-js/sql.js/releases/tag/v1.5.0)

- sqljs 1.5 릴리즈 - 2021-03-12에 있던 sqlite 3.35 릴리즈 적용
- sqlite 3.35 내용
    - Math function
    - Column removal
    - RETURNING processed rows for DELETE, INSERT and UPDATE
    - Materialized CTEs.

### [Spectacle 7: A React and JSX-Based Presentation Library](https://github.com/FormidableLabs/spectacle)

- 리액트 기반 프레젠테이션 라이브러리