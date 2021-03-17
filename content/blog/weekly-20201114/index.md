---
title: javascript weekly 2020-11-14
date: "2020-11-14T09:10:00.000Z"
description: "javascript weekly 2020-11-14"
tags: ["javascript"]
---

## 10 Insights From Adopting TypeScript At Scale
<a href="https://www.techatbloomberg.com/blog/10-insights-adopting-typescript-at-scale/" target="_blank">10 Insights From Adopting TypeScript At Scale</a>
- 블롬버그가 TS를 채택하면서 얻은 교훈
- js개발자가 2천명, v8기반으로 자체 빌드해서 얻은 이점

## Angular 11 Released
<a href="https://blog.angular.io/version-11-of-angular-now-available-74721b7952f7" target="_blank">Angular 11 Released</a>
- 앵귤러 11 릴리즈
	- 폰트 자동 인라인
	- 향상된 리포팅 및 로깅
	- 업데이트된 HMR 지원
	- 더 빨라진 빌드
	- 실험적인 웹팩 5 지원
	- IE 9, IE 10, IE Mobile 지원 중단
- 앵귤러 개발자 170만명 이상

## Babylon.js 4.2 Released: Powerful 3D Rendering Engine
<a href="https://babylonjs.medium.com/babylon-js-4-2-simplicity-reimagined-965f88d0fad" target="_blank">Babylon.js 4.2 Released: Powerful 3D Rendering Engine</a>
- 다양한 에디터 지원
	- https://playground.babylonjs.com/#M7MYT8#11
	- https://playground.babylonjs.com/#G3Q7GR#1
	- https://playground.babylonjs.com/#3TM0BZ#12
- Babylon React Native 지원
	- N-API를 통한 동기 통신
	- RN이 JSI를 사용하는 만큼, RN에서 사용될 땐 JSI 위에 N-API를 올림
	- RN의 헤르메스 엔진도 지원하지만, 아직 불완전
- glTF형식의 KTX + BasicUI 지원
	- jpeg을 능가하는 고급압축
- webXR 지원(컨트롤러 포함)

<hr>

# Quick bytes

## https://devblogs.microsoft.com/commandline/windows-terminal-preview-1-5-release/
- windows terminal preview 1.5 릴리즈
	- 완전한 하이퍼 링크 지원
	- 이모티콘 지원
	- 배경 이미지 설정 가능
- 1.4는 메인 버전으로 올라감

<hr>

# Code & Tools

## Mermaid: Markdown-'ish' Syntax for Generating Flowcharts, Sequence Diagrams, and More
<a href="https://mermaid-js.github.io/mermaid/#/" target="_blank">Mermaid: Markdown-'ish' Syntax for Generating Flowcharts, Sequence Diagrams, and More</a>
- 텍스트 to 다이어그램
- 마크다운스러운 표현

## ShareDB 1.5: Realtime Database Backend Based on Operational Transformation
<a href="https://github.com/share/sharedb" target="_blank">ShareDB 1.5: Realtime Database Backend Based on Operational Transformation</a>
- OT(Operational Transformation)기반 실시간 백엔드 디비
- 웹소켓을 통한 데이터 실시간 동기화
