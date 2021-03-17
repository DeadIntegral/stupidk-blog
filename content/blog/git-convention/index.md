---
title: git convention
date: "2020-02-04T23:50:00.000Z"
description: "git commit message convention"
tags: ["git"]
---

# intro
다음은 <a href="https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#-commit-message-guidelines" target="_blank">angular의 커밋 컨벤션</a>입니다. 다른 프로젝트에서도 충분히 훌륭한 에제입니다.

# Commit Message Format
각 커밋 메시지는 header, body, footer로 구성합니다.  
header는 type, scope, subject를 포함하는 특별한 타입입니다.  
```
<type>(<scope>): <subject>
<BLANK LINE>
<body>
<BLANK LINE>
<footer>
```

# Type
+ **build**: 빌드 시스템이나 외부 종속성에 영향을 주는 변경 사항 (예: gulp, brocoli, npm)
+ **ci**: CI 설정 파일 및 스크립트 변경(예: Travis, Circle, BrowserStack, SauceLabs)
+ **docs**: 문서만 변경
+ **feat**: 새로운 기능 추가
+ **fix**: 버그 수정
+ **perf**: 성능을 향상시키는 코드 변경
+ **refactor**: 버그를 수정하거나 기능을 추가하지 않는 코드 변경
+ **style**: 코드의 의미에 영향을 주지 않는 변경 사항(예: white-space, formatting, semi-colons)
+ **text**: 테스트 코드를 추가하거나, 기존 테스트 코드 수정

# Scope
scope란 영향을 받는 패키지(종속성)의 이름이어야 합니다.  
다음은 허용 가능한 scope 목록입니다.  
다음의 목록은 프로젝트마다 컨셉을 협의하면 좋을 것 같습니다.  
+ **animations**
+ **common**
+ **complier**
+ **core**
+ **elements**
+ **forms**
+ **http**

# Subject
변경 사항에 대한 간결한 설명을 적습니다.  
+ 현재 시제(change 대신 changed 혹은 changes)를 사용합니다.
+ 첫 글자를 대문자로 쓰지 않습니다.
+ 끝부분에 dot(.)을 쓰지 않습니다.

# Body
**subject**와 마찬가지로 명령형, 현재 시제를 사용합니다.