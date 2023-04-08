---
title: dev-weekly 2022-01-22
date: "2022-01-22T09:00:00.000Z"
description: "dev-weekly 2022-01-22"
tags: ["javascript", "node", "css"]
---

# CSS

### **[How to Make a Pure CSS 3D Package Toggle](https://css-tricks.com/how-to-make-a-pure-css-3d-package-toggle)**

- CSS로 3D 박스 애니메이션 만들기

### **[Make Beautiful Gradients](https://www.joshwcomeau.com/css/make-beautiful-gradients)**

- 그라디언트를 그냥 사용하면 중간에 회색지대가 생김
- HSL이나 HCL는 중간값도 같은 밝기를 유지하지만, 아직 HSL Inerpolation 지원 안됨
- 여러 중간값을 만들어서 매끄러운 hsl gradient를 만드는 생성기

### **[Responsive Image Gallery With Animated Captions](https://moderncss.dev/responsive-image-gallery-with-animated-captions)**

- 반응형 이미지 갤러리 만들기 (feat. 접근성)
    - object-fit : 반응형 이미지 스케일링
    - aspect-ratio : 일관된 이미지 사이즈
    - absolute position을 대체하는 CSS Grid 트릭
    - 애니메이션 효과를 위한 CSS transform (Ken Burns effect)
    - 터치 디바이스를 위한 핸들링
    - reduced motion 존중

### **[Accessible Heading Structure](https://www.a11yproject.com/posts/how-to-accessible-heading-structure)**

- accessible heading 을 만드는 조언들
- 접근성 도구 추천 - [https://wave.webaim.org/](https://wave.webaim.org/)

# Node

### **[Remix vs Next.js](https://remix.run/blog/remix-vs-next)**

- 리믹스 팀에서 작성한 Next와 Remix 비교
- 비교 방법이 공개되어있고, 공정하려고 노력

### **[structuredClone()](https://twitter.com/simonplend/status/1483789097734918152)**

- 노드17 부터 제공되는 딥클론.
- [https://developer.mozilla.org/en-US/docs/Web/API/structuredClone](https://developer.mozilla.org/en-US/docs/Web/API/structuredClone)

# Javascript

### **[A JavaScript-Flavored Introduction to Monads](https://github.com/getify/monio/blob/master/MONADS.md#fp--monads)**

- `You Don’t Know JS` 의 저자 카일 심슨의 모나드 글

### **[Deeply Copying Objects with `structuredClone()`](https://2ality.com/2022/01/structured-clone.html)**

- 인스턴스를 복사하면 일반 객체가 됨
- 함수, DOM 노드는 복사불가

### **[Deno 1.18 Released: The (Other) Modern JS/TS Runtime](https://deno.com/blog/v1.18)**

- Web Cryptography API 완성
- devtools 확장

### **Release**

- [https://eslint.org/blog/2022/01/eslint-v8.7.0-released](https://eslint.org/blog/2022/01/eslint-v8.7.0-released)
- [https://github.com/remarkjs/react-markdown/releases/tag/8.0.0](https://github.com/remarkjs/react-markdown/releases/tag/8.0.0)
- [https://github.com/ionic-team/capacitor/releases/tag/3.4.0](https://github.com/ionic-team/capacitor/releases/tag/3.4.0)
- [https://github.com/axios/axios/releases/tag/v0.25.0](https://github.com/axios/axios/releases/tag/v0.25.0)

### **[How to Extract Secrets from an Electron App](https://www.staszewski.me/how-to-extract-secrets-from-unsafe-electron-app/)**

- 일렉트론 빌드 결과물의 소스코드 확인하는 방법
- 중요한 값들은 빌드할 때 노출되지 않도록 주의하고, 프로덕션은 앱 콘솔 끄기

### **[Rockpack 2.0: An Alternative React App Builder](https://github.com/AlexSergey/rockpack)**

- CRA처럼 프로젝트 셋팅 시간을 감소시키는것이 목표
- SSR, Testing, ESLint 등도 기본 셋팅