---
title: javascript weekly 2020-02-08
date: "2020-02-08T08:30:00.000Z"
description: "javascript weekly 2020-02-08"
tags: ["javascript"]
---


# angular 9.0.0 release

<a href="https://blog.angular.io/version-9-of-angular-now-available-project-ivy-has-arrived-23c97b63cfa3" target="_blank">angular 9.0.0 이 릴리즈</a> 되었습니다. 지난 3년 중 가장 큰 업데이트 라고 합니다.  
마이그레이션 하는 방법은 angular8 lastest로 업데이트를 하고, 9로 업데이트 하라고 합니다.  

가장 큰 것은 역시 Ivy 컴파일러 및 런타임 입니다.
+ 보다 작은 번들(트리쉐이킹)
+ 테스트 퍼포먼스 향상
+ 디버깅 향상
+ CSS 클래스 및 스타일 바인딩 개선
+ type 검사 향상
+ 빌드 오류 개선
+ AOT를 통한 빌드 시간 개선
+ 국제화(i18n) 향상

# electron 8.0
<a href="https://www.electronjs.org/blog/electron-8-0" target="_blank">electron 8.0 이 릴리즈</a>되었습니다. 
크로미움 80, V8 8.0, Node.js 12.13 으로의 업그레이드를 포함합니다.	

# Javascript Build-in Decimal Proposal
<a href="https://github.com/littledan/proposal-decimal" target="_blank">Decimal type이 stage 0 이</a> 되었습니다.
bigInt 처럼 숫자 뒤에 문자(m)를 붙여서 사용합니다.  
ex) 0.1m + 0.2m // 0.3m

# Babel F# pipeline operator

<a href="http://codereform.com/blog/post/babel-fsharp-pipeline-operator/" target="_blank">Babel F# pipeline operator(|>)</a>는 선언적인 코드를 작성하기 위한 노력의 일환입니다.  
|> 문법에 대한 제안은 tc39에서도 <a href="https://github.com/tc39/proposal-pipeline-operator">의논중</a>인 문법으로 Smart Style과 F# 스타일로 나뉘어 집니다.  

```javascript
const result = 5
    |> add(10, ?)
    |> mul(2, ?)
    |> subtract (?, 3);

console.log("The value is:", result); // prints: "The value is: 27"
```

# Building an accessible autocomplete control
vanilla 로 만든 <a href="https://adamsilver.io/articles/building-an-accessible-autocomplete-control/" target="_blank">accessible autocomplete</a>입니다.
사용자의 입력 처리(키보드 인풋)부터, onblur, Tab, select된 메뉴 강조, 메뉴 스크롤, 클릭을 통한 메뉴 선택, 필터링 등 다양한 부분을 직접 구현합니다.  

# You Dont Need Momentjs
You Dont Need JQuery 에 이어 이번엔 <a href="https://github.com/you-dont-need/You-Dont-Need-Momentjs" target="_blank">Momentjs</a> 입니다.
chart를 통한 cheat sheet 로 각 라이브러리들을 비교해주고, 똑같은 기능을 수행하기 위한 각 라이브러리의 예시 코드를 제공해줍니다.  

이미 momentjs 를 대체하려고 나온 많은 라이브러리가 있고, 많은 이동이 있었지만 기존의 moment생태계가 너무 컸나봅니다.  
또한 ECMA가 발전하면서 Built-in 으로 처리 가능한 부분도 생기며, 늦게 등장한 라이브러리일 수록 경량화 되어가고 있습니다.

# Implementing Basic 2D Physics in JavaScript
<a href="https://martinheinz.dev/blog/15" target="_blank">Physics의 JS 구현</a>입니다.
안타깝게도 중간에 레이텍 수식이 깨진 부분이 있습니다.  
중력과 충돌에 대한 부분을 그림을 통해 쉽게 설명해줍니다.


# CheerpJ 2.0 released
<a href="https://medium.com/leaningtech/cheerpj-2-0-released-381f6d03e4e" target="_blank">CheerpJ 2.0</a>은 레거시 자바 애플리케이션을 WASM + JS로 변환하여 HTML5 애플리케이션으로 변환하여 통합시키는 것을 목적으로 합니다.

# BARETEST, An extremely minimalistic alternative to Jest
<a href="https://volument.com/baretest" target="_blank">BARETEST</a>는 빠르고 간단한 test runner입니다. 우리가 테스트를 할 때, re-ordering, mocking, snapshotting이 항상 필요하진 않습니다.  BARETEST에서는 그 부분을 뺀 대신, 높은 성능 향상을 보여줍니다.

# x-spreadsheet
<a href="https://github.com/myliang/x-spreadsheet">x-spreadsheet</a> 가 이제는 cdn 으로도 제공됩니다. 또한 언어팩도 추가되었습니다.