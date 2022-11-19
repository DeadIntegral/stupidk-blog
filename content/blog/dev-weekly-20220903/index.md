---
title: dev-weekly 2022-09-03
date: "2022-09-03T10:20:00.000Z"
description: "dev-weekly 2022-09-03"
tags: ["javascript", "css", "node",]
---

# CSS

### **[Meet the top layer: a solution to z-index:10000](https://developer.chrome.com/blog/what-is-the-top-layer)**

- dialog의 장점들
    - document flow 바깥에 위치하고, 때문에 z-index에는 영향을 받지 않음
    - 스타일 지정 가능한 `::backdrop` 슈도 엘리먼트가 존재
    - 각 엘리먼트와 `::backdrop` 은 새로운 스택킹 컨텍스트를 생성

### **[Using Grid Named Areas to Visualize (and Reference) Your Layout](https://css-tricks.com/using-grid-named-areas-to-visualize-and-reference-your-layout)**

- grid-template-areas 를 이용해 사용자 지정 영역 생성
    
    ```css
    .grid-container {
      grid-template-areas:
        "head head head"
        "left main right"
        "left main right"
        "foot foot foot";
    }
    ```
    
- 커스텀 네임은 자동으로 <custom-ident>-start|end 4개를 자동으로 획득

### **[20 principles I learned from 10 years of developing software](https://dev.to/ondrejsevcik/20-principles-i-learned-from-10-years-of-developing-software-5354)**

- 10년간 소프트웨어 개발을 하며 배운 20가지 원칙
    - 5. 유즈 케이스의 80% 해결 - 모든 사람의 문제를 해결할 수 없음
    - 10. 메모하기 - 기억할 것이라고 생각하는것은 스스로에게 거짓말 하는 것

# Node

### **[Tinybench: A Tiny and Simple Benchmarking Library](https://github.com/tinylibs/tinybench)**

- 의존성 없고 작고 가볍고 심플한 벤치마킹 도구

### **[Heroku Reveals Roadmap; Will Drop Free Plans](https://blog.heroku.com/next-chapter)**

- 퍼블릭 로드맵 - [https://github.com/heroku/roadmap](https://github.com/heroku/roadmap)
- 프리 플랜을 중단하고 비활성 계정 삭제
- 학생 및 비영리 단체 지원
- 오픈소스 지원

### **[Dynamoose 3.0](https://github.com/dynamoose/dynamoose/releases/tag/v3.0.0)**

- AWS dynamoDB 모델링 도구 3.0 릴리즈
- 다량의 브레이킹 체인지
    - aws-sdk v3, …etc

# Javascript

### **[JSON Crack: Visualize JSON Data in Graph Form](https://jsoncrack.com/editor)**

- JSON Data를 넣으면 그래프로 만들어주는 도구

### **[jQuery 3.6.1 is here](https://blog.jquery.com/2022/08/26/jquery-3-6-1-maintenance-release/)**

- v3.6.0 이후 18개월만의 릴리즈

### **[Understanding React's `useMemo` and `useCallback`](https://www.joshwcomeau.com/react/usememo-and-usecallback/)**

- useMemo 예시와 컴포넌트를 분리하는 등 다양한 대안 제시
- useCallback은 useMemo의 문법 설탕

### **[In-Browser Compression and Decompression with the Compression Streams API](https://developer.chrome.com/blog/compression-streams-api/)**

- gzip, deflate 압축 및 해제가 가능한 CompressionStream API

### **[Partytown 0.7: Run Third Party Scripts in a Web Worker](https://github.com/BuilderIO/partytown/releases/tag/v0.7.0)**

- 써드 파티 라이브러리의 메인 스레드의 작업을 웹워커로 배치하는 도구 Partytown 0.7 릴리즈

### **[Sandpack: Component Toolkit for Creating Your Own Live Running Code Editing Experience](https://sandpack.codesandbox.io/)**

- 코드샌드박스 샌드팩 리액트 패키지.
- 코드 에디터를 컴포넌트로 제공