---
title: dev-weekly 2022-04-09
date: "2022-04-09T21:50:00.000Z"
description: "dev-weekly 2022-04-09"
tags: ["javascript", "css", "node"]
---

# CSS

### **[Variable Fonts in Real Life: How To Use and Love Them](https://evilmartians.com/chronicles/variable-fonts-in-real-life-how-to-use-and-love-them)**

- 여러 폰트 파일을 하나의 파일로 대체 가능한 Variable Font
- 실제 사용 시 장점
- 다크 테마일 때 물리적인 이유로 인해 달라지는 wehgith

### **[Designing a Better Infinite Scroll](https://www.smashingmagazine.com/2022/03/designing-better-infinite-scroll)**

- pagenation의 장단점, Infinite scroll의 장단점
- 둘을 결합하는 방법, infinite scroll 개선사례

### **[How To Match HTML Elements With an Indeterminate State](https://www.stefanjudis.com/today-i-learned/how-to-match-html-elements-with-an-indeterminate-state)**

- 선택 이전을 나타내는 `:indeterminate`
- checkbox에 적용 시 클릭 이전의 상태

# Node

### [Node 18's upcoming test runner system](https://nodejs.org/download/nightly/v18.0.0-nightly20220403561885152e/docs/api/test.html)

- 노드18부터는 built-in test runner 추가
    
    ```tsx
    const test = require('node:test');
    const assert = require('assert');
    
    test('synchronous passing test', (t) => {
      // This test passes because it does not throw an exception.
      assert.strictEqual(1, 1);
    
    });
    ```
    
- 3월24일 이후 nightly build 로 사용 가능
- [https://fusebit.io/blog/node-testing-comes-to-core/](https://fusebit.io/blog/node-testing-comes-to-core/)

### ****[Announcing AWS Lambda Function URLs: Built-in HTTPS Endpoints for Single-Function Microservices](https://aws.amazon.com/ko/blogs/aws/announcing-aws-lambda-function-urls-built-in-https-endpoints-for-single-function-microservices/)****

- 람다에 https 엔드포인트를 추가하고, 선택적으로 CORS 헤더 구성 가능
- `Content-type` 등 주의사항 및 적합한 사례
    - API Gateway의 고급기능이 필요하지 않은 공용 엔드포인트

### **[Kafka.js 1.16.0: A Modern Apache Kafka Client](https://github.com/tulios/kafkajs/releases/tag/v1.16.0)**

- Kafkajs 1.16 릴리즈

### [Fastify 3.28.0: The Fast and Low Overhead Web Framework](https://github.com/fastify/fastify/releases/tag/v3.28.0)

- Fastify 3.28.0 릴리즈

# Javascript

### **[Announcing Rome Formatter: Super Fast JavaScript Formatting](https://rome.tools/blog/2022/04/05/rome-formatter-release)**

- Rome 프로젝트의 Formatter 공개
- 코드의 중간에 이슈가 있을 때 뒷부분도 포맷팅하지 않는 이슈 해결
- Prettier보다 약 9~12배 성능 향상

### **[Writing Redux Reducers in Rust](https://fiberplane.dev/blog/writing-redux-reducers-in-rust/)**

- Reducer를 Rust - WASM 으로 작성하기
- 로직을 호출 할 때 마다 직렬화해서 WASM과 통신해야하는 코스트
- TS 에 Rust-Reducer 노출 및 호출
- 장점
    - Rust가 immutable을 강제할 것이기 때문에 우연한 뮤테이션을 걱정하지 않음
    - Immer를 사용하는 효과지만 의존성이 추가되지 않음

### **[Announcing RedwoodJS 1.0 and $1M Funding](https://tom.preston-werner.com/2022/04/04/redwood-v1-and-funding.html)**

- RedwoodsJS 1.0 출시, $1M 투자

### Release

- [https://astro.build/blog/astro-1-beta-release/](https://astro.build/blog/astro-1-beta-release/)
- [https://reactnative.dev/blog/2022/03/30/version-068](https://reactnative.dev/blog/2022/03/30/version-068)

### **[ShadowRealms: An ECMAScript Proposal for a Better `eval()`](https://2ality.com/2022/04/shadow-realms.html)**

- 현재 컨텍스트와 별도의 컨텍스트에서 임의의 JS 코드를 실행하는 새로운 방법 - stage3

### **[How to Test Component Interactions with Storybook](https://storybook.js.org/blog/test-component-interactions-with-storybook/)**

- 컴포넌트는 데이터와 사용자 인터랙션에 연관되어 있고 개발자들은 자동화된 테스트에 의존. 대부분의 테스트는 Node 및 JSDOM 기반이고 cli에서 시각적 UI 를 디버그해야함
- 이를 개선하는 스토리북 인터랙션 테스트 워크플로
- feat. Testing Library, Jest, MSW, Playwright
- CI 에서 테스트 러너 실행하기, 크로마틱을 통한 시각적 테스트 결합

### **[React Libraries to Use in 2022](https://www.robinwieruch.de/react-libraries/)**

- 리액트 개발을 도와주는 라이브러리들

### **[Preview.js: Preview UI Components Instantly in Your IDE](https://previewjs.com/)**

- 리액트, 뷰의 프리뷰를 제공해주는 도구 VSCode, JetBrain IDE 호환