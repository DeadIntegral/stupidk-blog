---
title: dev-weekly 2022-12-17
date: "2022-12-17T10:40:00.000Z"
description: "dev-weekly 2022-12-17"
tags: ["javascript", "css", "node"]
---
# CSS

### **[CSS image()](https://12daysofweb.dev/2022/css-image)**

- `url()` 은 몇 가지 제약사항이 있어서 새롭게 도입된 함수
- image fragments(이미지의 특정 부분 -px, %- 그리기), Directionality(ltr, rtl), fallback color
- 이미지 색칠하기 - `background-image: image(hsl(210 47% 20% / .75)), url("images/my-image.jpg");` 와 같이 사용하여 url의 이미지 위에 레이어 씌우는 트릭

### **[Accessible color palette generator](https://venngage.com/tools/accessible-color-palette-generator)**

- 웹 접근성 지침 가이드에 맞는 색상 팔레트 생성기

# Node

### **Node Weekly most popular links**

- **[Tao of Node: On Design, Architecture and Best Practices](https://alexkondov.com/tao-of-node/)**
- **[Popular Node.js Patterns and Tools to Reconsider](https://practica.dev/blog/popular-nodejs-pattern-and-tools-to-reconsider/)**
- **[JavaScript and Node Testing Best Practices: 2022 Edition](https://github.com/goldbergyoni/javascript-testing-best-practices#readme)**
- **[Best Practices for Creating a Modern npm Package](https://snyk.io/blog/best-practices-create-modern-npm-package/)**

# Javascript

### **[Announcing SvelteKit 1.0](https://svelte.dev/blog/announcing-sveltekit-1.0)**

- 스벨트킷이 다른 도구들과 다른점
- 같이 사용할 수 있는 도구(생태계) 및 배포 가능한 영역(adapter-node)

### **[Dr. Axel Tackles Two Proposals: Iterator Helpers and Set Methods](https://2ality.com/2022/12/iterator-helpers.html)**

- ECMA proposal Iterator Helper가 어떻게 작동하고, 기존의 Iterator와 어떻게 다른지, 어떤 충돌이 있고 어떻게 해결 가능한지 설명한 아티클

### **[jQuery 3.6.2 Released](https://blog.jquery.com/2022/12/13/jquery-3-6-2-released/)**

- 사용자  정의 CSS에 대해 오류 발생하던 부분 수정
- `:has()` 로 인한 문제점에 대해서 크롬, CSSWG에서 수정. JQuery에서는 브라우저에서 지원하는 셀렉터인지 검증하는 로직 추가

### **[Optimize Interaction to Next Paint](https://web.dev/optimize-inp/)**

- Interaction to Next Paint는 사용자가 이용하는 동안 발생하는 모든 인터랙션의 반응성을 평가하는 메트릭
- 이벤트 콜백 최적화, 프레젠테이션 지연 최적화

### **Release**

- **[Chart.js 4](https://github.com/chartjs/Chart.js/discussions/10977)**

- **[SWR 2.0: Improved React Hooks for Data Fetching](https://swr.vercel.app/blog/swr-v2)**
    - React 18 대응
    - 빌드 타겟 ES2018로 변경 (IE 11 드랍)을 통한 향상된 성능 및 보다 작은 번들 사이즈
    - 새로운 기능인 `useSWRMutation`, 새로운 모델 `Optimistic UI`
    - Mutate Multiple Keys, Preserving Previous State