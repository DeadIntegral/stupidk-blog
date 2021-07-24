---
title: dev-weekly 2021-07-24
date: "2021-07-24T09:00:00.000Z"
description: "dev-weekly 2021-07-24"
tags: ["javascript", "node", "css", "go"]
---

# CSS

### [Sometimes, a Billion Laughs Aren't so Funny — Improving CSS Variables in WebKit](https://engineering.widen.com/blog/Improving-CSS-Variables-in-WebKit)

- 웹킷에서 CSS Variable 개선하기
    - bilion lol, fallback, relative-path, :visited(미해결)

### [Towards Richer Colors on the Web](https://darker.ink/writings/Towards-richer-colors-on-the-Web)

- 우리가 볼 수 있는 색상, 웹에서 표현가능한 색상
- blink 엔진의 렌더 파이프라인과 현재의 문제 - Skia(다중 플랫폼 그래픽 라이브러리)에 데이터 전달하기까지 - 와 개선안
- [bit.ly/lifeofapixel](http://bit.ly/lifeofapixel) 79번째 슬라이드가 핵심

### [Build Complex CSS Transitions using Custom Properties and cubic-bezier()](https://css-tricks.com/build-complex-css-transitions-using-custom-properties-and-cubic-bezier)

- cubic-bezier() 와 Custom Property들을 사용해서 복잡한 transition 만들기

### [Maintaining End-To-End Quality With Visual Testing](https://www.smashingmagazine.com/2021/07/maintaining-end-to-end-quality-visual-testing)

- 기존의 복잡한 테스팅이 잡지 못하는 UI 이슈도 존재, 비쥬얼 테스팅의 장점 어필
    - 픽셀별비교 ⇒ 오탐지를 할 수 있음
    - AI활용 ⇒ 이미지를 비교하여 변경된곳, 같은곳을 별도로 표시

# Node

### [Notion API: Getting Started with Notion's JavaScript SDK](https://www.sitepoint.com/notion-api-javascript-sdk/)

- JS sdk를 이용하여 노션 API 시작하기

### [ncc: Compile a Node Project Into a Single File](https://github.com/vercel/ncc)

- 노드 모듈을 모든 종속성을 포함한 단일 파일로 컴파일 하는 cli

### [Mineflayer: A High Level API for Creating Minecraft Bots](https://github.com/PrismarineJS/mineflayer)

- 노드로 마인크래프트 봇 만드는 도구

### [Nativefier: Make Any Web Page a Desktop Application](https://github.com/nativefier/nativefier)

- 웹사이트 주소 입력하면 데스크탑앱으로 만들어주는 도구
- 일렉트론 래퍼

# Go

### [An Interesting Go Memory Issue?](https://boyter.org/posts/interesting-go-memory-issue/)

# Javascript

### [JetBrains' 2021 Developer Ecosystem Survey Results](https://www.jetbrains.com/lp/devecosystem-2021/)

- 183개국 31,743명의 개발자 설문조사 결과
- [https://www.jetbrains.com/lp/devecosystem-2021/javascript/](https://www.jetbrains.com/lp/devecosystem-2021/javascript/)

### [https://domenicobrz.github.io/webgl/projects/SSRefractionDepthPeeling/](https://domenicobrz.github.io/webgl/projects/SSRefractionDepthPeeling/)

- threejs로 만든 유리 세공

### [Abracadabra: JS and TS Refactoring Tool for VS Code](https://marketplace.visualstudio.com/items?itemName=nicoespeon.abracadabra#abracadabra)

- 코드 리팩토링해주는 도구
- 같은 동작을 하는 다른 구조 ⇒ 가독성 향상 및 유지보수 비용 절약