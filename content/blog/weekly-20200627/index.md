---
title: javascript weekly 2020-06-27
date: "2020-06-27T09:00:00.000Z"
description: "javascript weekly 2020-06-27"
tags: ["javascript"]
---

# Lessons Learned Refactoring Optional Chaining Into a Large Codebase
<a href="https://lea.verou.me/2020/06/refactoring-optional-chaining-into-a-large-codebase-lessons-learned/" target="_blank">Lessons Learned Refactoring Optional Chaining Into a Large Codebase</a>

```
//Ternary
foo? foo.bar : defaultValue
foo?.bar || defaultValue
foo?.bar ?? defaultValue

// Array checking
if (foo.length > 3) {
	foo[2]
}
foo?.[2]

// Feature detection
if (element.prepend) element.prepend(otherElement);
element.prepend?.(otherElement);

...
```

# What's Coming in TypeScript 4? 
<a href="https://httptoolkit.tech/blog/whats-coming-in-typescript-4" target="_blank">What's Coming in TypeScript 4? </a>
- ts4.0 beta release(2020.06.25) 8월 릴리즈 예정
- https://devblogs.microsoft.com/typescript/announcing-typescript-4-0-beta/

<hr>

# Quick bytes
## 크롬85
<a href="https://developers.google.com/web/updates/2020/06/devtools" target="_blank">크롬85</a>
- css in js 편집가능
- lighthouse 6.0
- 네트워크 패널에 service worker response 추가
- wasm 소스 오픈 시 byte code offset 표기
- ...

## 엔지니어링 블로그 모음
<a href="https://engineeringblogs.xyz/" target="_blank">엔지니어링 블로그 모음</a>

<hr>


# Code & Tools
## https://github.com/tannerlinsley/react-query/releases/tag/v2.0.0 리액트 쿼리 2.0 릴리즈
- 비동기 데이터 fetch, cache, update를 위한 hook
- Transport/protocol/backend agnostic data fetching (REST, GraphQL, promises, whatever!)
- Auto Caching + Refetching (stale-while-revalidate, Window Refocus, Polling/Realtime)
- Parallel + Dependent Queries
- Mutations + Reactive Query Refetching
- ...

## https://www.bryanbraun.com/checkboxland/ 체크박스랜드. 렌더링은 체크박스만 함.

