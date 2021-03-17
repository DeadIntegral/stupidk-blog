---
title: javascript weekly 2020-12-12
date: "2020-12-12T09:00:00.000Z"
description: "javascript weekly 2020-12-12"
tags: ["javascript"]
---

## The 'Import on Interaction' Pattern
<a href="https://addyosmani.com/blog/import-on-interaction" target="_blank">The 'Import on Interaction' Pattern</a>
- 레이지 로드에 관한 Addy Osmani의 포스트
- 로그인 연동의 번들은 무거우니까 버튼을 누를때만 가져오기
- ssr이라고 하더라도 hydration이 끝나기 전가지 인터랙션 못함
	- => 처음엔 모든 클릭을 추적하는 작은 번들(https://github.com/google/jsaction)을 제공하기
- 페이지를 정적 형태로 변환하기
- ...

## Get Ready to Up Your (Google) Apps Script
<a href="https://developers.googleblog.com/2020/12/get-ready-to-up-your-apps-script.html" target="_blank">first release candidate of Snowpack v3.0</a>
- 구글에서 apps script IDE라는, 새로운 온라인 IDE를 공개
- https://developers.google.com/apps-script/guides/dashboard
- https://www.google.com/script/start/

## Deno 1.6 Released: You Can Now Build Executables
<a href="https://deno.land/posts/v1.6" target="_blank">Deno 1.6 Released: You Can Now Build Executables</a>
- deno 1.6.0이 릴리즈. 1.0 이후 가장 큰 피쳐
- 스탠드얼론 바이너리 빌드
	- 아직은 언스테이블
	- 용량이 40MB에 육박
	- 아직 웹워커, dynamic import, v8 flag 등 몇 가지 제약 존재
- Built-in Deno Language Server
- arm64 실험적 지원

<hr>

# Quick Releases and etc

## https://code.visualstudio.com/updates/v1_52
- vscode 1.52 릴리즈

## https://www.infoq.com/news/2020/12/nativescript-joins-openjs/
- 네이티브 스크립트가 openJS Foundation 조인

## https://github.com/settings/appearance
- 깃헙 다크 모드 출시

## https://rome.tools/funding/
- Babel, Yarn을 만들었던 분이 Rome 툴킷 펀딩과 진행중인 작업

<hr>

# Tutorials

## How to Create a Favicon That Changes Automatically
<a href="https://css-tricks.com/how-to-create-a-favicon-that-changes-automatically/" target="_blank">How to Create a Favicon That Changes Automatically</a>
- 동적인 파비콘 만들기
- reference
	- 댄의 useInterval https://overreacted.io/making-setinterval-declarative-with-react-hooks/

<hr>

# Code & Tools

## Electron React Boilerplate 2.0: A Foundation for Scalable Cross-Platform Apps
<a href="https://github.com/electron-react-boilerplate/electron-react-boilerplate/releases/tag/v2.0.0" target="_blank">Electron React Boilerplate 2.0: A Foundation for Scalable Cross-Platform Apps</a>
- 일렉트론 보일러 플레이트 2.0.0 릴리즈
- redux drop
- react-refresh, webpack5, electron11 로 마이그레이션
- 디렉토리 이름 변경
	- app은 src로, resources는 asset

## SiriWave: The Apple Siri Waveform Replicated in Pure JavaScript
<a href="https://jsdiff.dev/" target="_blank">SiriWave: The Apple Siri Waveform Replicated in Pure JavaScript</a>
- 애플 시리 웨이브 애니메이션(canvas)
- 녹음 및 재생 시의 효과


## Markdown Editor 2.0: A Simple, React-Powered Markdown Editor with Preview
<a href="https://github.com/uiwjs/react-md-editor" target="_blank">Markdown Editor 2.0: A Simple, React-Powered Markdown Editor with Preview</a>
- 리액트에 붙이는 markdown editor
- https://uiwjs.github.io/react-md-editor/
