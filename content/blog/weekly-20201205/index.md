---
title: javascript weekly 2020-12-05
date: "2020-12-05T10:00:00.000Z"
description: "javascript weekly 2020-12-05"
tags: ["javascript"]
---

## WMR: A Tiny All-in-One Development Tool for Modern Web Apps
<a href="https://github.com/preactjs/wmr" target="_blank">WMR: A Tiny All-in-One Development Tool for Modern Web Apps</a>
- preact 팀에서 만든 올인원 패키지
	- import "packages" from npm without installation
	- Smart bundling and caching for npm dependencies
	- Lightning-fast JSX support
	- CSS Modules
	- Static file serving with hot reloading of CSS and images

## first release candidate of Snowpack v3.0
<a href="https://www.snowpack.dev/posts/2020-12-03-snowpack-3-release-candidate" target="_blank">first release candidate of Snowpack v3.0</a>
- 스노우팩 3.0 후보 첫 릴리즈
- skypack cdn을 이용한 npm install 제거
- esbuild 도입

## Chrome 88
<a href="https://blog.chromium.org/2020/12/chrome-88-digital-goods-lighting.html" target="_blank">Chrome 88</a>
- WebXR: AR Lighting Estimation
- :not(.a + .b .c) 과 같이 복잡한 not() 지원
- COOP, COEP 뒤에 SharedArrayBuffer 추가
- SharedArrayBuffer, arrayBuffer 에서 사용하는 Atomics 지원
- FTP 지원 종료

<hr>

# Quick Releases

## https://github.com/aframevr/aframe/releases/tag/v1.1.0
- a-frame 1.1.0 릴리즈
- WebXR compositor layers API
- WebXR DOM Overlays
- WebXR hand tracking API proposal

## https://dev.to/arcanis/yarn-2-4-log-filters-audits-better-warnings-49io
- yarn 2.4 릴리즈

## https://mail.openjdk.java.net/pipermail/nashorn-dev/2020-November/007597.html 
- Nashorn 15.0 릴리즈.
- 독립형 버전
- java15 required

<hr>

# Tutorials

## Puppeteer vs Selenium vs Playwright, A Browser Automation Speed Comparison
<a href="https://blog.checklyhq.com/puppeteer-vs-selenium-vs-playwright-speed-comparison/" target="_blank">Puppeteer vs Selenium vs Playwright, A Browser Automation Speed Comparison</a>
- 사과와 오렌지의 비교에 가깝지만, 그래도 왜 비교하게 되었는지에 대한 이유
- 어떤 환경에서 어떠한 시도로 측정했는지와 그 결과에 대한 포스트

<hr>

# Code & Tools

## JSONEditor: A Component for Viewing and Editing JSON
<a href="https://github.com/josdejong/jsoneditor" target="_blank">JSONEditor: A Component for Viewing and Editing JSON</a>
- json editor
- http://jsoneditoronline.org/ 라이브 버전
- tree-mode 에서는 양쪽 json을 diff 가능
- 외부 파일 가져오기, 공유, 정렬, 필터 등 다양한 기능 제공

## JsDiff: A Visual Comparison of JavaScript Library Metrics
<a href="https://jsdiff.dev/" target="_blank">JsDiff: A Visual Comparison of JavaScript Library Metrics</a>
- npm에서의 다운로드 숫자
- 구글 트렌드
- 깃헙 오픈이슈, pr 분석, 스타 수 등을 시각화


## Compressor.js: Client-Side Image Compressor
<a href="https://fengyuanchen.github.io/compressorjs/" target="_blank">Compressor.js: Client-Side Image Compressor</a>
- client side 이미지 압축 라이브러리 - jpeg quality 를 이용
- https://github.com/antelle/wasm-image-compressor
	- png 압축 라이브러리
	- libimagequant, libpng, zlib등을 사용했고, Emscripten을 통해 wasm으로 빌드


## noUiSlider: Lightweight Range Slider with Full Multi-Touch Support
<a href="https://refreshless.com/nouislider/examples/" target="_blank">noUiSlider: Lightweight Range Slider with Full Multi-Touch Support</a>
- 종속성 없는 ui 슬라이더
- 스텝 지정 기능(스텝 단위로 움직이는)
- 각 슬라이더의 start 설정(커넥트와 연계하여 최소지점)
- label제공 및 label 클릭 시 그 지점으로 애니메이션 이동
- 툴팁 제공 등 다양한 기능
