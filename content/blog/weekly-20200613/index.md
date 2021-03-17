---
title: javascript weekly 2020-06-13
date: "2020-06-13T09:30:00.000Z"
description: "javascript weekly 2020-06-13"
tags: ["javascript"]
---

# An ECMAScript Proposal: Logical Assignment Operators
<a href="https://2ality.com/2020/06/logical-assignment-operators.html" target="_blank">An ECMAScript Proposal: Logical Assignment Operators</a>
- ||=, &&=, ??= 추가 프로포절
```javascript
// recap
a || b // a ? a : b
a && b // !a ? a : b
a ?? b // a !== undefined && a !== null ? a : b
// proposed
a ||= b // a || (a = b)
a &&= b // a && (a = b)
a ??= b // a ?? (a = b)
```

# Quick bytes
## VS Code May 2020 has been released
<a href="https://code.visualstudio.com/updates/v1_46" target="_blank">VS Code May 2020 has been released</a>
- 사이드 메뉴와 하단 메뉴를 드래그해서 원하는 위치로 옮길 수 있습니다.
- github remote
- commonJS auto imports + Add all missing imports source action

## front-end development learning pathway
<a href="https://developer.mozilla.org/en-US/docs/Learn/Front-end_web_developer" target="_blank">front-end development learning pathway</a>

## https://titlerun.xyz/ 브라우저 타이틀 바에서 재생되는 게임



<hr>

# 이후의 링크는 node weekly

<hr>

# Prisma 2.0: Next Gen Database Wrangling from Node
<a href="https://www.prisma.io/blog/announcing-prisma-2-n0v98rzc8br1" target="_blank">Prisma 2.0: Next Gen Database Wrangling from Node</a>

# Two Ways of Rate Limiting an Express App
<a href="https://eugene.coding.blog/rate-limiting-an-express-app" target="_blank">Two Ways of Rate Limiting an Express App</a>
- 사용자마다 요청 제한을 거는 방법에 대한 기본 컨셉
- RxXpress를 사용해 스트림을 간단히 쓰로틀 걸기


# Modules and Tools
## https://github.com/sindresorhus/terminal-image 터미널에 이미지 그리기
## https://github.com/11ways/janeway 콘솔 repl인데 클릭 가능(객체 누르면 펴짐)
## https://github.com/felixrieseberg/windows95 윈95 일렉트론