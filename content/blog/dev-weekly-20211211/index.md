---
title: dev-weekly 2021-12-11
date: "2021-12-11T10:00:00.000Z"
description: "dev-weekly 2021-12-11"
tags: ["css", "node", "javascript"]
---

# CSS

### **[The 2021 Web Almanac — CSS](https://almanac.httparchive.org/en/2021/css)**

- 웹 생태계에 있어서 CSS의 사용 경향, 변화, 패턴에 대해 설명해주는 아티클

### **[Defensive CSS](https://ishadeed.com/article/defensive-css/)**

- 스타일이 깨지지 않도록 방어해주는 css property들
- `flex-wrap`, `overscroll-behavior`, `CSS Variable Fallback`, `scrollbar-gutter` 등

### **[Cross-Fading Any Two DOM Elements Is Currently Impossible](https://jakearchibald.com/2021/dom-cross-fade)**

- 한 영역에서 글자를 다른 글자로 변경하기
- opacity가 0.5, 0.5가 만나면 0.75가 되버리기 때문에 오작동
- `cross-fade()`, canvas - `globalCompositeOperation`, `mix-blend-mode`

### **[Open Props: Sub-Atomic Styles](https://open-props.style/)**

- CSS consistent design 모음

# Node

### **[serious improvements to its code search functionality](https://github.blog/2021-12-08-improving-github-code-search/)**

- 깃헙 코드 검색 기능 개선 - 베타 사용자 모집

### **[Chalk 5.0](https://github.com/chalk/chalk/releases/tag/v5.0.0)**

- 5.0 릴리즈, pure ESM으로 변경. TS 이용자는 4 를 이용할듯

### **[graphql-request: A Minimal GraphQL Client for Node and Browsers](https://github.com/prisma-labs/graphql-request)**

- minified 18.8kb, gziped 6kb의 가벼운 노드, 브라우저용 GraphQL 클라이언트

### **[Ink 3.2: React, but for Building Interactive CLI Apps](https://github.com/vadimdemedes/ink/releases/tag/v3.2.0)**

- 리액트 17 호환

# Javascript

### **[How We Cut 99% of Our JavaScript with Qwik and Partytown](https://www.builder.io/blog/how-we-cut-99-percent-js-with-qwik-and-partytown)**

- JS Main Thread 에서 실행되지 않아도 되는 코드들을 worker로 보내서 성능 향상

### **[**Github a new 'lists' feature in beta**](https://github.blog/changelog/2021-12-09-lists-are-now-available-as-a-public-beta/)**

- 깃헙의 새로운 star list

### **[November edition of VS Code](https://code.visualstudio.com/updates/v1_63)**

- 페이지 내 검색 기능 강화
- Unicode highlighting - 보이지 않는 유니코드 문자들 강조 표시
- NPM Scripts view improvements
- TypeScript 4.5
- markdown preview 내장(탭에서 우클릭)

### **[Tailwind CSS v3.0 Released](https://tailwindcss.com/blog/tailwindcss-v3)**

- Just in Time 향상
- 스크롤 스냅 API

### **[OpenLayers 6.9: High Performance Frontend Mapping Library](https://github.com/openlayers/openlayers/releases/tag/v6.9.0)**

- 동적 지도를 페이지에 배치하는 라이브러리 v6.9 릴리즈