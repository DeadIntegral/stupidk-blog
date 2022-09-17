---
title: dev-weekly 2022-09-17
date: "2022-09-17T16:00:00.000Z"
description: "dev-weekly 2022-09-17"
tags: ["javascript", "css", "node",]
---
# CSS

### **[Building the Main Navigation for a Website](https://web.dev/website-navigation)**

- 사이트의 nav를 접근성 맞추기 아티클
- `aria-current` 현재 페이지를 의미론적으로 전달
- safari의 voiceOver는 의도적으로 ul의 list-style: none일 때 list의미를 제거. 명시적으로 `role="list"` 적기
- `aria-labelledby` 를 통해 기존 label 참조
- 좁은 뷰포트에서 nav 대체하기 - `aria-expanded` , `aria-controls`, `aria-label`

### **[WebKit Features in Safari 16.0](https://webkit.org/blog/13152/webkit-features-in-safari-16-0)**

- 사파리 16의 기능들
- WebPush, AVIF 포맷, WebAuth(FIDO), apple pay, container query, shared worker
- 접근성 개선, 애니메이션 개선, overscroll behavior

### **[CSS line-height](https://markodenic.com/css-line-height)**

- line height의 기본값(normal)은 1.2
- 단위 없는 숫자는 font size * line height 만큼의 px영역, 사용할 수 있는 단위는 px, em, rem, pt, cm 등, %는 font-size에 대한 백분율
- 접근성 지침에선 font-size의 1.5배 이상을 권장

### **[A Moment of Pure CSS](https://codepen.io/ivorjetski/pen/yLjeqgb)**

- JS, Image를 사용하지 않고 마크업으로 그려낸 풍경화

# Node

### **[Best Practices for Creating a Modern npm Package](https://snyk.io/blog/best-practices-create-modern-npm-package/)**

- 2022년에 NPM 패키지를 만드는 베스트 프랙티스
- cjs, esm 셋팅, 패키지 생성, 테스팅, 보안검사 등에 이르는 스텝 바이 스텝

### **[Favicons 7.0: A Favicon Generation Library](https://github.com/itgalaxy/favicons/releases/tag/v7.0.0)**

- Favicon 생성기 7.0 릴리즈
- Jimp대신 Sharp 사용, maskable 아이콘, TS도입

### [September 22nd 2022 Security Releases](https://nodejs.org/en/blog/vulnerability/september-2022-security-releases/)

- 9월 22일 여러 문제(high severity)로 인해 Nodejs 보안 릴리즈. 18.x, 16.x, 14.x

# Javascript

### **[MemLab: A Framework for Finding JavaScript Memory Leaks](https://engineering.fb.com/2022/09/12/open-source/memlab/)**

- JS 메모리 테스트 프레임워크(자동 메모리 릭 감지)
- [https://github.com/facebookincubator/memlab](https://github.com/facebookincubator/memlab)
- memlab을 만든 이유, 작동 방식, 기능 소개

### **[JavaScript APIs You Don’t Know About](https://www.smashingmagazine.com/2022/09/javascript-api-guide/)**

- 잘 알려지지 않은 Web API들
    - Visibility API
    - Web Share API
    - Broadcast Channel API
    - Internationalization API

### **[The *Seventh* Way to Call a Function Without Parentheses](https://portswigger.net/research/the-seventh-way-to-call-a-javascript-function-without-parentheses)**

- 괄호 없이 함수를 호출하는 7번째 방법
    
    ```jsx
    alert`1337`
    throw onerror=alert,1337
    Function`x${'alert\x281337\x29'}x```
    'alert\x281337\x29'instanceof{[Symbol['hasInstance']]:eval}
    valueOf=alert;window+''
    x=new DOMMatrix;matrix=alert;x.a=1337;location='javascript'+':'+x
    // or any DOMXSS sink such as location=name
    ```
    

### **[What’s New with HTML Forms in 2022?](https://css-tricks.com/whats-new-with-forms-in-2022/)**

- `form.requestSubmit()` 사파리16지원. submit()과 다르게 validation 실행
- `submitter` 제출된 이벤트 속성에 접근

### **[The Secret of Successfully Using Multi Window WebGL Canvas](https://itnext.io/the-secret-of-successfully-using-multi-window-webgl-canvas-5a2d05555ad1)**

- OffscreenCanvas, sharedWorker를 이용하여 애니메이션 노드를 창 옮겨다니게 하기
- OffscreenCanvas 의 오너십을 worker에게 이전 및 소유권 이전을 여러번 하기 위한 트릭

### **[Theatre.js 0.5: Hackable Motion Design for the Web](https://www.theatrejs.com/blog/theatre-05-is-out)**

- 웹 모션 디자인 편집기 0.5 릴리즈
- 키프레임 인라인 편집

### ****[Disabled JavaScript turns off native lazy loading](https://www.stefanjudis.com/today-i-learned/disabled-javascript-turns-off-native-lazy-loading/)****

- 자바스크립트를 비활성화 하면 `loading="lazy"` 가 작동하지 않음
- 사이트가 페이지의 마크업에 전략적으로 이미지를 배치하여 세션 전체에서 사용자의 스크롤 위치를 추적할 수 있기 때문에, 추적 방지 조치

# Etc

### **[Set up a new Mac, Fast](https://cpojer.net/posts/set-up-a-new-mac-fast)**

- yarn, jest의 개발자가 전하는 맥을 빠르게 셋팅하는 팁

[https://www.stefanjudis.com/today-i-learned/disabled-javascript-turns-off-native-lazy-loading/](https://www.stefanjudis.com/today-i-learned/disabled-javascript-turns-off-native-lazy-loading/)