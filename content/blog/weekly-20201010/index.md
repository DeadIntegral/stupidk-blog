---
title: javascript weekly 2020-10-10
date: "2020-10-10T08:00:00.000Z"
description: "javascript weekly 2020-10-10"
tags: ["javascript"]
---

# RSLint: A Super Fast JS Linter Written in Rust
<a href="https://github.com/RDambrosio016/RSLint" target="_blank">RSLint: A Super Fast JS Linter Written in Rust</a>
- rust로 작성된 성능 중심의 jslint

# Writing JavaScript Tools in Other Languages – A New Trend?
<a href="https://2ality.com/2020/10/js-plus-other-languages.html" target="_blank">Writing JavaScript Tools in Other Languages – A New Trend?</a>
- 다른 언어로 작성된 js 도구들
- 다른 언어를 사용하는 이유

# Volta: Install, Run, and Manage JavaScript Tools Quickly
<a href="https://github.com/volta-cli/volta" target="_blank">Volta: Install, Run, and Manage JavaScript Tools Quickly</a>
- 다른 언어로 작성된 js 도구들
- 다른 언어를 사용하는 이유

<hr>

# Quick bytes

## https://web.dev/camera-pan-tilt-zoom/
- 크롬 87부터는 카메라 PTZ(pan, tilt, zoom) control을 API 로 제공

## https://discord.com/invite/angular
- 앵귤러 공식 디스코드 출범

## https://code.visualstudio.com/updates/v1_50
- 리눅스 ARMv7, ARM64 에서 vscode 이용 가능
- https://marketplace.visualstudio.com/items?itemName=ms-vscode.vscode-js-profile-flame 을 설치하면 시피유, 램 리얼타임 메트릭 제공 및 엣지나 크롬을 이용중일 경우 DOM nodes, relayouts, restyles 도 제공
<hr>

# The File System Access API: Simplifying Access to Local Files
<a href="https://web.dev/file-system-access/" target="_blank">The File System Access API: Simplifying Access to Local Files</a>
- 로컬 파일과 상호작용(수정 및 저장까지)하는 API
- https://wicg.github.io/file-system-access/

# Go, WebAssembly, HTTP Requests and Promises
<a href="https://withblue.ink/2020/10/03/go-webassembly-http-requests-and-promises.html" target="_blank">Go, WebAssembly, HTTP Requests and Promises</a>
- golang WASM을 js와 상호작용 시키는 포스팅
	- js의 promise를 사용하기 위한 go의 코드
	- http request 구현 - 네트워크 호출이 차단되므로 gorutine에서 실행해야함.
	- streaming 구현

<hr>

# Code & Tools

## https://blogs.windows.com/msedgedev/2020/10/01/microsoft-edge-tools-vscode/
- vscode 안에 웹브라우저 개발자 도구 삽입

## https://github.com/johnmichel/Library-Detector-for-Chrome
- like wappalyzer. 사이트에서 어떤 라이브러리 사용중인지 표시해주는 익스텐션