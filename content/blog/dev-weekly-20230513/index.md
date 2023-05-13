---
title: dev-weekly 2023-05-13
date: "2023-05-13T12:40:00.000Z"
description: "dev-weekly 2023-05-13"
tags: ["javascript", "css", "node", "etc"]
---

# CSS

### **[Future CSS: Anchor Positioning](https://kizu.dev/anchor-positioning-experiments/)**

- position: absolute 로 배치된 요소가 다른 요소의 위치 등에 영향을 받게 만들 수 있음.
- 앵커 포지셔닝으로 만든 예제들
    - HTML, CSS만으로 만든 fold 가능한 트리 등

### **[Don’t use custom CSS scrollbars](https://ericwbailey.website/published/dont-use-custom-css-scrollbars)**

- 스크롤바를 커스텀하면 안되는 이유들
    - 고해상도 대비 등 사용자 커스텀에 대응을 하지 않는 스크롤바 색상
    - 외적 일관성 (장치의 다른 모든 서비스에서와 다른 스크롤바)
    - 스크롤 가능하다는 별도의 어포던스가 필요할 수 있음

# Node

### **[Practical Guide To Not Blocking The Event Loop](https://www.bbss.dev/posts/eventloop/)**

- 더 많은 노드 띄우기 - 이로 인한 문제점
- 동기식 작업을 비동기(Promise)로 변환하는 예제
- 다른 스레드로 오프로드 하기(Worker)

### **[GitHub Actions: All Actions will run on Node16 instead of Node12](https://github.blog/changelog/2023-05-04-github-actions-all-actions-will-run-on-node16-instead-of-node12/)**

- 깃헙 액션의 Node12는 5월18일 부터 Node16으로 대체될 예정

### **[Notion-to-MD: Convert Notion Pages to Markdown](https://github.com/souvikinator/notion-to-md)**

- 노션 페이지의 블록, 블록 목록을 마크 다운으로 컨버팅 해주는 도구

# Javascript

### **[Next.js 13.4](https://nextjs.org/blog/next-13-4)**

- 스테이블한 App Router 제공 - 스테이블의 의미는 앱 라우터의 핵심이 프로덕션 준비가 된 것. 작업 완료는 아님. page router도 지원.
- Turbopack 베타
- [https://nextjs.org/docs](https://nextjs.org/docs) 로 문서 병합

### **[The JavaScript Ecosystem Is Delightfully Weird](https://fly.io/blog/js-ecosystem-delightfully-wierd/)**

- JS 생태계에 대한 단상 feat. 번들러
- 발전해온 역사적 배경, 현대에는 JSX, TS 등으로 작성하고 결과물이 JS일 뿐 JS로 작성 하지 않는 이상함
- 최근 번들러들에 의해서는 다른 언어의 프레임워크와 유사한 RSC

### **[Svelte PR: **TS to JSDoc Conversion**](https://github.com/sveltejs/svelte/pull/8569)**

- Svelte 타입을 TS에서 JSDoc으로 변환 하는 PR
- [https://news.ycombinator.com/item?id=35892250](https://news.ycombinator.com/item?id=35892250) 해당 PR은 해커뉴스에서 1위를 하고, 리치 해리스가 컨텍스트 공유
    - 타입 안정성을 포기하는 것이 아니라 타입 선언을 옮기는 것. TS의 모든 이점은 그대로 유지

### **[ES2023 introduces new array copying methods to JavaScript](https://www.sonarsource.com/blog/es2023-new-array-copying-methods-javascript/)**

- toSorted(), toReversed(), toSpliced, with() 메서드를 통해 원본 배열을 변경하지 않고 해당 작업의 결과물로 새로운 배열 반환하기
- 배열의 각 값들을 복사하는 것이기 때문에, 값이 참조면 효력없음.

### **[Fake Windows 11 in Svelte](https://win11-svelte.vercel.app/)**

- Svelte로 만든 가짜 windows11. 에뮬레이터나 OS가 아니라 유사한 UI
- https://github.com/yashash-pugalia/win11-svelte

### **[React Canaries: Enabling Incremental Feature Rollout Outside Meta](https://react.dev/blog/2023/05/03/react-canaries)**

- React에서 공식 지원하는 Canary 릴리스 채널 공개

# ETC

### **[Introducing Baseline](https://web.dev/introducing-baseline/)**

- baseline이란? - 기능이나 API 가 웹에서 사용하기 안전한지 한눈에 확인가능한 지표.
- 메이저 브라우저의 최신 두 버전에서 지원되는 모든 기능은 baseline에 포함
- web.dev와 mdn에 baseline 추가.
- [https://web.dev/baseline/](https://web.dev/baseline/)

### **[The ongoing defence of frontend as a full-time job](https://christianheilmann.com/2023/05/09/the-ongoing-defence-of-frontend-as-a-full-time-job/)**

- 시장의 오해와 프론트엔드 개발자가 하는 업무.

### **[HTML CheatSheet](https://htmlcheatsheet.com/)**

- html 치트시트. 태그, 스트럭쳐, 컬러 피커, 특수 문자(hover 시 html entity) 등 다양한 시트를 인터랙션으로 제공

### **Release**

- [elementary 2.0](https://www.notion.so/2023-05-13-514d38001b1a4c89b0ed9e6d9428b0f4)
- [htmlparser2 9.0](https://github.com/fb55/htmlparser2/releases/tag/v9.0.0)