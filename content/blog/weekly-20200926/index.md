---
title: javascript weekly 2020-09-26
date: "2020-09-26T08:30:00.000Z"
description: "javascript weekly 2020-09-26"
tags: ["javascript"]
---

# Vime: A Customizable Media Player Built with Web Components
<a href="https://vimejs.com" target="_blank">Vime: A Customizable Media Player Built with Web Components</a>
- 리액트, 앵귤러, 뷰, 스벨트 등을 지원
- 크로스 브라우징(IE는 제외) - 동일한 UI 지원
- I18N 등 다양한 기능 제공


# V8 Release 8.6
<a href="https://v8.dev/blog/v8-release-86" target="_blank">V8 Release 8.6</a>
- V8 8.6 릴리즈
- toString 을 Torque로 작성하여 최대 75% 성능 향상
- WASM to JS Call 의 성능 향상


# Deno 1.4 Released
<a href="https://deno.land/posts/v1.4" target="_blank">Deno 1.4 Released</a>
- Node Security 

<hr>

# Quick bytes

## https://devblogs.microsoft.com/typescript/announcing-typescript-4-1-beta/
- TS 4.1 베타


## https://reactjs.org/blog/2020/09/22/introducing-the-new-jsx-transform.html
- React 17 JSX - import React 생략
	```
	import React from 'react';
	```

## https://v8.dev/blog/slack-tracking
- v8의 slack trace
- 새로운 객체를 생성할 때, 실제 사용할 것 보다 더 큰 크기를 할당(8개의 추가 프로퍼티)하고, 일정 시간 후에 사용하지 않는 공간을 비우는 방법
- 그 일정 시간이 되기 전에 프로퍼티를 추가하면 그건 더 빠르게 추가
<hr>

# How to Visualize Data Structures in VS Code
<a href="https://addyosmani.com/blog/visualize-data-structures-vscode/" target="_blank">How to Visualize Data Structures in VS Code</a>
- vscode extension - Debug Visualizer 포스트
- fetch 데이터에 대한 시각화도 가능

<hr>

# Code & Tools
## A console for mobile browsers.
<a href="https://github.com/balazsbotond/urlcat" target="_blank">A console for mobile browsers.</a>
- 중복되는 /제거, encodeURIComponent 실행 등 url 작성 도와주는 도구
	```
	const API_URL = 'https://api.example.com/';
	const path = '/user'
	//이와 같이 있더라도 하나의 '/'만 남기고 제거
	```

## 11 Top Node ORMs, Query Builders and Database Libraries in 2020
<a href="https://www.prisma.io/dataguide/database-tools/top-nodejs-orms-query-builders-and-database-libraries-in-2020" target="_blank">11 Top Node ORMs, Query Builders and Database Libraries in 2020</a>
- 프리즈마에서 선정한 라이브러리 11선
- Popularity, Repo Activity, Support, Maturity & Stability 에 대한 평가