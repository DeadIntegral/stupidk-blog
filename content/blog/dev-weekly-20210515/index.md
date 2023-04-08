---
title: dev-weekly 2021-05-15
date: "2021-05-15T09:30:00.000Z"
description: "dev-weekly 2021-05-15"
tags: ["javascript", "css", "node"]
---

# CSS, Deno

## CSS

### **[Creating Colorful, Smart Shadows](https://www.kirupa.com/html5/creating_colorful_smart_shadows.htm)**

- `background: inherit;`, `filter: drop-shadow(0px 0px 10px rgba(0, 0, 0, 0.50)) blur(20px);` 를 이용하여 이미지의 색상을 유지하는 그림자 생성하기

### **[Auditing Design Systems for Accessibility](https://www.deque.com/blog/auditing-design-systems-for-accessibility)**

- 접근성을 고려해서 디자인 시스템을 만드는 방법

### **[CSS Cuboid Generator](https://codepen.io/jh3y/pen/MWJdqBo)**

- CSS 직육면체 생성기 feat.codepen

### **[CSS DNA 🧬](https://codepen.io/shadow-scientist/pen/eYgPjxX)**

- HTML과 CSS로만 만들어진 아티클

---

## Deno

### **[Deno 1.10 Released](https://deno.com/blog/v1.10)**

- Web Storage API 추가. localStorage 와 sessionStorage 지원
- remote import map 지원
- 향상된 test runner - 처음부터 다시 작성
    - [https://caspervonb.medium.com/rewriting-denos-testing-tools-b5f8801bc567](https://caspervonb.medium.com/rewriting-denos-testing-tools-b5f8801bc567)
- 웹워커 직렬화된 모든 데이터를 허용하도록 변경
    - [https://developer.mozilla.org/en-US/docs/Web/API/Web_Workers_API/Structured_clone_algorithm](https://developer.mozilla.org/en-US/docs/Web/API/Web_Workers_API/Structured_clone_algorithm) 을 이용
- WASM 메모리 공유 활성화

---

# Javascript

### **[Angular 12 Released](https://blog.angular.io/angular-v12-is-now-available-32ed51fbfd49)**

- Ivy 로의 완전한 전환(view engine 사용 안함) - Ivy everywhere
- 레거시 i18n Message Id 변환
- nullish Coalescing 지원
- 앵귤러 학습을 위한 가이드 문서들 제작
    - ex) [https://angular.io/guide/content-projection](https://angular.io/guide/content-projection)
- IE 11에 대한 지원 중단 경고 메시지 포함. 13에서 지원 중단

### **['Babel Is Used by Millions, So Why Are We Running Out of Money?'](https://babeljs.io/blog/2021/05/10/funding-update.html)**

- 바벨의 자금 조달 상황
    - 바벨 개발자 중 일부는 정규직으로 돌아가기도 함
    - [https://opencollective.com/babel](https://opencollective.com/babel)
    - [https://github.com/sponsors/babel](https://github.com/sponsors/babel)

### **Quick Bits**

- Azure Static Web Apps
    - [https://azure.microsoft.com/en-us/blog/develop-production-scale-modern-web-apps-quickly-with-azure-static-web-apps/](https://azure.microsoft.com/en-us/blog/develop-production-scale-modern-web-apps-quickly-with-azure-static-web-apps/)
    - vscode 플러그인

## Articles, Opinions & Tutorials

### **[Why JWT Should Not Be Your Default for Sessions](https://evertpot.com/jwt-is-a-bad-default/)**

- jwt의 장점은 확장성. 그만한 규모의 웹이 얼마나 있는가?
- 간단한 구현이 있는데 복잡한것이 왜 디폴트인가?

## Code & Tools

### **[Elder.js: An 'SEO-First' Svelte-Based Framework](https://elderguide.com/tech/elderjs/)**

- SEO-First 프레임워크 Elder의 최근 큰 변화
- SSR & SSG 성능 지표