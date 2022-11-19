---
title: dev-weekly 2022-05-14
date: "2022-05-14T20:00:00.000Z"
description: "dev-weekly 2022-05-14"
tags: ["javascript", "css", "node"]
---
# CSS

### **[State of CSS 2022](https://web.dev/state-of-css-2022)**

- Google IO 에서 볼 수 있는 현재와 미래의 웹 스타일링
- 현재의 모습 - layer, container-query, accent-color, COLRv1 Font ...
- `grid-template-rows: masonry;`, `prefers-reduced-data`, `:toggle`

### **[Learn CSS Subgrid](https://ishadeed.com/article/learn-css-subgrid/)**

- 서브그리드가 필요한 예제와, 서브그리드를 통한 해결

### **[Can you use a WebP file as an Open Graph Protocol image?](https://www.ctrl.blog/entry/webp-ogp.html)**

- Open Graph Protocol에서 페이스북, 트위터 등의 문서는 WebP를 지원하지 않는다고 적혀있지만 실제로는 지원

### **[Iris Door (Hexagonal) - Pure CSS](https://codepen.io/josetxu/pen/RwxzwEa)**

- Hover시 6개의 삼각형으로 문이 닫히는 애니메이션

# Node

### **[A Community Group for Web-Interoperable JavaScript Runtimes](https://blog.cloudflare.com/introducing-the-wintercg/)**

- WinterCG 설립 발표
- 브라우저는 항상 origin을 기반으로 작동, cloudflare worker, nodejs, deno는 origin이 존재하지 않음. ⇒ 브라우저가 아닌 JS환경에서 표준 웹 API의 상호운용성(interop)에 중점
- 기존 웹 API의 최소 집합. 자체적인 독립 API를 출시하진 않을 것.

[https://engineering.fb.com/2022/05/11/open-source/jest-openjs-foundation/](https://engineering.fb.com/2022/05/11/open-source/jest-openjs-foundation/)

- 메타의 오픈소스 Jest가 OpenJS Foundation으로 이동

### **[What's Involved in Running a Ransomware Attack in a Node Module](https://charliegerard.dev/blog/ransomware-script-node-module/)**

- JS Module로 랜섬웨어 공격하는법 - 교육 목적의 글
- 쉘 스크립트를 만들고, 노드에서 쉘 스크립트를 호출하기, 남들이 다운받게 만들기

### **[Kafka.js 2.0: A Modern Apache Kafka Client](https://github.com/tulios/kafkajs/releases)**

- 4년만의 첫 메이저 업데이트

# Javascript

### **[Using Google's CrUX to Compare Performance of JS Frameworks](https://www.smashingmagazine.com/2022/05/google-crux-analysis-comparison-performance-javascript-frameworks/)**

- 구글 크롬의 CoreWebVital 메트릭을 통한 지표 확인 feat.Wappalyzer
- 상위 사이트만 확인하면 Vue가 React보다 LCP, CLS 등에서 좋게 나타남
- Wix로 만든 사이트도 React 지표에 포함됨. 성능 프로파일 미스터리의 원인

### **[Thoughts on React's Forthcoming `useEvent` Hook](https://typeofnan.dev/what-the-useevent-react-hook-is-and-isnt/)**

- 리렌더링 되더라도 함수를 다시 만들지 않는 `useEvent`

### **[Deno turns 4 today!](https://twitter.com/deno_land/status/1525119512277725184)**

- Deno 의 4번째 생일

### **[TypeScript 4.7 Release Candidate](https://devblogs.microsoft.com/typescript/announcing-typescript-4-7-rc/)**

- TS 4.7 RC
- package.json에서 exports, imports, 자체참조
- module detection, Instantiation Expressions ...

### **[Get to Know Your Browser's Performance Profiler](https://blog.atomrc.dev/p/js-performance-profiling/)**

- 브라우저의 퍼포먼스 프로파일러 보는법
- 모질라 문서 - [https://profiler.firefox.com/docs/#/](https://profiler.firefox.com/docs/#/)