---
title: javascript weekly 2020-09-12
date: "2020-09-12T09:30:00.000Z"
description: "javascript weekly 2020-09-12"
tags: ["javascript"]
---

# Playwright 1.4: Fast and Reliable Cross-Browser Testing
<a href="https://github.com/microsoft/playwright/releases/tag/v1.4.0" target="_blank">Playwright 1.4: Fast and Reliable Cross-Browser Testing</a>
- 1.4 릴리즈
- playwright-cli 추가
- 사용자의 행동을 기록하여 코드로 변환해줌.

# How Browsers May Throttle requestAnimationFrame
<a href="https://mattperry.is/writing-code/browsers-may-throttle-requestanimationframe-to-30fps" target="_blank">How Browsers May Throttle requestAnimationFrame</a>
- RAF는 브라우저에 의해 쓰로틀링이 있을 수 있습니다. (주로 IOS 에서)

<hr>

# Quick bytes

## https://code.visualstudio.com/updates/v1_49
vscode 8월 릴리즈
- 기존 코드는 냅두고 새로 변경된 부분에만 스타일(prettier같은) 적용
- auto attach : --inspect 하지 않아도 자동으로 디버그 모드
- TS Convert Optional Chaning Refactoring 드래그하면 옵셔널 체이닝으로 리팩토링

## https://developers.google.com/web/tools/chrome-devtools/javascript/breakpoints
debugger remind.  
break point는 다음의 경우에 걸 수 있음.
- 코드 라인
- 조건부 코드 라인
- DOM
- XHR
- event listener
- exception (코드가 아닌 throw를 만나면 자동으로 멈추도록)
- function (함수 이름에 걸면 호출될 때 마다 멈춤)

<hr>

#
# Rendering React on the Edge with Flareact and Cloudflare Workers
<a href="https://blog.cloudflare.com/rendering-react-on-the-edge-with-flareact-and-cloudflare-workers/" target="_blank">Rendering React on the Edge with Flareact and Cloudflare Workers</a>
- flareact라는 프레임워크. 클라우드 플레어 워커(0ms 콜드 스타트)에서 리액트를 렌더링 및 캐싱

# Creating Extensions for Visual Studio Code: An Introduction
<a href="https://www.syncfusion.com/blogs/post/creating-extensions-for-visual-studio-code-a-complete-guide.aspx" target="_blank">Creating Extensions for Visual Studio Code: An Introduction</a>
- vscode extenstion 만들기


# How cdnjs Migrated to Serverless with Workers KV
<a href="https://blog.cloudflare.com/migrating-cdnjs-to-serverless-with-workers-kv/" target="_blank">How cdnjs Migrated to Serverless with Workers KV</a>
- 클라우드 플레어의 cdnjs 서비스를 Worker-KV와 서버리스로 마이그레이션한 스토리


# Symbolic Computation in JavaScript with Math.js
<a href="https://blog.klipse.tech/javascript/2020/09/10/symbolic-computation-math-js.html" target="_blank">Symbolic Computation in JavaScript with Math.js</a>
- 복소수, 행렬, 방정식 등을 연산하도록 해주는 라이브러리
```
math.evaluate('bar(x,y) = (x+y)(x-y)', scope)
math.evaluate('bar(10,5)', scope)
// 75
```