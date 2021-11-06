---
title: dev-weekly 2021-10-30
date: "2021-10-30T17:00:00.000Z"
description: "dev-weekly 2021-10-30"
tags: ["javascript", "node", "css"]
---

# CSS

### **[Respecting Users’ Motion Preferences](https://www.smashingmagazine.com/2021/10/respecting-users-motion-preferences)**

- js에서 적용할 땐 `window.matchMedia('(prefers-reduced-motion: reduce)')`
- 애니메이션을 완전히 제거하는것이 아님. 제거할 경우 갑작스러운 전환이 발생해 더 좋지 않을 수 있음.
- 재생빈도가 낮은 기기의 경우 애니메이션 제거가 나을 수 있음 ⇒  `(update: slow)` 를 같이 사용

### **[We Analyzed 425,909 Favicons](https://iconmap.io/blog#before-we-begin---favicon-best-practices)**

- favicon은 IE5 릴리즈와 함께 탄생
- 파비콘에 대한 통계 데이터

# Node

### **[A Comprehensive Guide to Error Handling in Node](https://www.honeybadger.io/blog/errors-nodejs/)**

- Node의 오류는 무엇인지와 오류의 타입별 설명

### **[Prisma 3.4.0 Released: The Popular 'Next Gen' ORM and Toolset](https://github.com/prisma/prisma/releases/tag/3.4.0)**

- PostgreSQL 14지원

# Javascript

### **[Chrome's New Feature to Record and Replay User Flows](https://developer.chrome.com/docs/devtools/recorder/)**

- 크롬 카나리에 레코더와 리플레이 기능 추가
- 레코딩된 데이터 수정 가능

### **[Angular 13 Released](https://blog.angular.io/angular-v13-is-now-available-cce66f7bc296)**

- 뷰엔진 사용 불가
- 컴포넌트 API 간소화
- IE 11 지원 종료

### **[Microsoft Brings (More) JavaScript to Excel](https://techcrunch.com/2021/11/02/microsoft-brings-javascript-to-excel/)**

- 엑셀에 JavaScript API 제공

### **[Announcing TypeScript 4.5 RC](https://devblogs.microsoft.com/typescript/announcing-typescript-4-5-rc/)**

- 프로젝트 로드 속도 향상
- JSX Attribute 자동완성

### [V8 release v9.7](https://v8.dev/blog/v8-release-97)

- 플래그 없이 사용 가능한 새로운 두 배열 함수(findLast, findLastIndex)

### **[Popular 'coa' NPM library hijacked to steal user passwords](https://www.bleepingcomputer.com/news/security/popular-coa-npm-library-hijacked-to-steal-user-passwords/)**

- NPM 다운로드 900만, 1400만인 Command-Option-Argument와 RC 하이잭킹. 이전의 us-parser-js 와 유사한 형태

### [리코일 0.5.0 릴리즈](https://github.com/facebookexperimental/Recoil/releases/tag/0.5.0)

### [퍼펫티어 11.0.0 릴리즈](https://github.com/puppeteer/puppeteer/releases/tag/v11.0.0)

### **[Depp: Check `npm` Modules for Unused and Duplicate Dependencies Fast](https://github.com/CryogenicPlanet/depp)**

- npm modules 에서 사용하지 않는 종속성 찾아주는 도구. go로 제작

### **[Detox: 'Gray Box' End-to-End Testing and Automation Framework for Mobile Apps](https://github.com/wix/Detox)**

- 모바일 앱, RN 을 지원하는 E2E 테스트 및 자동화 도구

# Etc

### [메타버스에 대한 글](https://m.clien.net/service/board/park/16652597?po=1&sk=title&sv=%25EB%25A9%2594%25ED%2583%2580%25EB%25B2%2584%25EC%258A%25A4&groupCd=&pt=0)