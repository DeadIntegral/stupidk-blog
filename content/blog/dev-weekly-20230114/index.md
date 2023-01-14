---
title: dev-weekly 2023-01-14
date: "2023-01-14T16:20:00.000Z"
description: "dev-weekly 2023-01-14"
tags: ["javascript", "node"]
---
# Node

### **[A Comparison of Node.js Job Schedulers](https://deadsimplechat.com/blog/best-nodejs-schedulers/)**

- 이 문서에서 말하는 Job Scheduler의 정의
- 몇가지 평가 기준을 바탕으로 깃헙에서 스타 높은 프로젝트 비교 (비교 기준을 만족하는 샘플 코드)
    - Persistence - 프로그램이 다시 시작된 뒤에도 재설정되지 않는지
    - Horizontal Scaling - 여러 호스트에서 job multiple processor를 지원하는지
    - 중복 실행 방지 - 다중 프로세스, 다중 스레드에서 실행하더라도 하나만 실행되는지

### **[I wish JSON5 was more popular](https://evertpot.com/json5/)**

- npm에서 JSON5를 채택하면 좋겠다는 글
- [https://www.npmjs.com/package/json5](https://www.npmjs.com/package/json5)

### **[Build a Serverless ChatGPT SMS Chatbot with OpenAI and Node](https://www.twilio.com/blog/sms-chatbot-openai-api-node)**

- OpenAI API를 이용하여 ChatGPT와 같은 챗봇 만들기

### **[publint: Lint if a Package is Published Correctly](https://publint.dev/)**

- 패키지를 입력하면 패키지의 package.json을 린팅하는 도구
- [https://publint.dev/rules](https://publint.dev/rules)

### Release

- [node-mysql2 3.0 릴리즈](https://github.com/sidorares/node-mysql2/releases/tag/v3.0.0) (작성당시 3.0.1)

# Javascript

### **[The State of JS 2022](https://2022.stateofjs.com/ko-KR/)**

- 앵귤러 만족도 42%, 솔리드 만족도 90%
- 모바일장치 - Tauri 만족도 91%, 일렉트론 사용량 35.2% RN 사용량 35.1%
- 최다적용기술 - vite, 최고만족도 - vite, 최고관심도 - vite

### **[Is TypeScript Worth It?](https://news.ycombinator.com/item?id=34359504)**

- 정적 타이핑은 좋지만, TS가 개발자에게 부가시키는 추가 작업의 양이 많다는 글로 시작된 토론
- Typescript PM Rosenwasser 의 응답

### **[The Gotcha of Unhandled Promise Rejections](https://jakearchibald.com/2023/unhandled-rejections/)**

- for await 이 reject promise를 만나면 이를 포함하는 함수가 throw처리가 되는 이슈
- Promise.all 을 통해 처리하는 방법
    - 더미 핸들러를 추가하는 방법(직접 만들기, Promise.allSettled 사용하기)

### **[Everything About React's 'Concurrent Mode' Features](https://blog.codeminer42.com/everything-you-need-to-know-about-concurrent-react-with-a-little-bit-of-suspense/)**

- Reeact 기본 방식에서의 문제점과 컨커런트 모드로 어떻게 해결하는지 설명
- 컨커런트 모드에 대한 자세한 내용

### **[Using GitHub Copilot for Unit Testing?](https://www.strictmode.io/articles/using-github-copilot-for-testing)**

- 코파일럿에게 유닛 테스트 작성시키기
- 코파일럿의 구현이 마음에 들지 않을 수 있지만, 테스트 코드 통과시킬정도면 충분하다는 스탠스

### **[Structura.js: Lightweight Library for Immutable State Management](https://giusepperaso.github.io/structura.js/)**

- immer와 유사하지만, 런타임 대신 컴파일 시간에만 TS를 활용하여 고정

### **[Mafs: React Components for Interactive Math](https://mafs.dev/guides/get-started/hello-f-x)**

- 인터랙션 가능한 수학 그래프 리액트 컴포넌트