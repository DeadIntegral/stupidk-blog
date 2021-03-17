---
title: javascript weekly 2020-02-22
date: "2020-02-22T08:30:00.000Z"
description: "javascript weekly 2020-02-22"
tags: ["javascript"]
---

# Fixing Memory Leaks in Web Applications
<a href="https://nolanlawson.com/2020/02/19/fixing-memory-leaks-in-web-applications/" target="_blank">웹 앱의 메로리 누수 고치기</a> 라는 포스트로, 일반적으로 메모리 릭을 일으키는 코드와 그에 대한 해결방안을 제시해줍니다.  
또한 chrome devtools를 이용하여 leak이 발생중인지 확인하는 방법 또한 가르쳐 줍니다.

# TypeScript 3.8 Released
<a href="https://devblogs.microsoft.com/typescript/announcing-typescript-3-8/" target="_blank">TS 3.8이 릴리즈</a>되었습니다.
+ export * as ns Syntax : import처럼 export도 단일 진입점 문법을 쓸 수 있게 되었습니다.(es2020)
+ Top-Level await : async 함수 밖에서도 await을 사용 가능합니다.
+ "Fast and Loose" Incremental Checking : TS가 다른 파일에 영향을 줄 수 있는지 추적하고, 가능한 많은 정보를 메모리에 담아 재사용합니다.
이 외에도 다양한 추가 사항이 있습니다.

# The Official Redux Template for Create React App v1.0 
<a href="https://github.com/reduxjs/cra-template-redux/releases/tag/v1.0.0" target="_blank">Release note</a>  
create-react-app에 redux 템플릿이 추가되었습니다.
```
npx create-react-app my-app --template redux
```

# GitExplorer: Find the Right git Commands To Use
<a href="https://gitexplorer.com/" target="_blank">Git Command Explorer</a>  
깃에서 내가 하고 싶은 명령을 순차적으로 선택하면, 그에 맞는 깃 커맨드를 입력해주는 서비스입니다.  
치트시트와 다르게 명령어를 모르는 상태에서 액션 기반으로 찾는다는 점이 큰 장점입니다.  
화면 좌 상단에서 속도 조절이 가능합니다.  

# A Practical Introduction to GeoJSON with Node
<a href="http://thecodebarbarian.com/a-practical-introduction-to-geojson-with-node-js.html" target="_blank">geoJSON</a>의 사용법을 간단히 소개합니다.

+ geoJSON이란 위치정보를 갖는 점을 기반으로 지형을 표현하는 <a href="https://tools.ietf.org/html/rfc7946">공개 표준 형식</a>입니다.