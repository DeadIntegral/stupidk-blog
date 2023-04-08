---
title: dev-weekly 2021-02-13
date: "2021-02-13T09:00:00.000Z"
description: "dev-weekly 2021-02-13"
tags: ["javascript", "css", "node", "web", "typescript", "deno"]
---

# Deno, CSS, Repl.it

### **Deno Module Visualizer**
<a href="https://deno-visualizer.danopia.net/" target="_blank">Deno Module Visualizer</a>
- deno 모듈 디펜던시를 시각화 해주는 도구

<hr>

### **he importance of `@font-face` source order when used with preload**
<a href="https://nooshu.github.io/blog/2021/01/23/the-importance-of-font-face-source-order-when-used-with-preload/" target="_blank">he importance of `@font-face` source order when used with preload</a>
- font face preload에서 발생할 수 있는 이슈와 성능 최적화에 대해 다루는 글

### **An Interactive Guide to CSS Transitions**
<a href="https://www.joshwcomeau.com/animation/css-transitions/" target="_blank">An Interactive Guide to CSS Transitions</a>
- timing functions 들의 잔상을 남겨서 시간대마다 얼마나 빠르게 움직였는지 확인 가능한 아티클
- 베지어 곡선에 대한 설명과 timing functions 에 대한 설명 포함
- 각 애니메이션를 직접 조작해볼 수 있도록 제공

### **Managing CSS Z-Index In Large Projects**
<a href="https://www.smashingmagazine.com/2021/02/css-z-index-large-projects/" target="_blank">Managing CSS Z-Index In Large Projects</a>
- 큰 프로젝트에서 z-index관리를 어떻게 할까에 관한 글
- css-in-js로 변수들을 만들고 거기에 숫자들 담아서 관리하는 컨셉
- 이 아티클의 내용은 css variable로도 충분히 재현 가능.

<hr>

### **Hosting Apps with Always On**
<a href="https://blog.repl.it/alwayson" target="_blank">Hosting Apps with Always On</a>
- repl always 출시. 웹 IDE에 hosting, package managing, https 등 제공
- 설명에는 db 등도 제공해준다고 함

<hr>

# Node

### **System Information Library for Node.JS**
<a href="https://github.com/sebhildebrandt/systeminformation" target="_blank">System Information Library for Node.JS</a>
- CPU, Memory 등 시스템 정보를 보여주는 라이브러리

### **Researcher hacks over 35 tech firms in novel supply chain attack**
<a href="https://www.bleepingcomputer.com/news/security/researcher-hacks-over-35-tech-firms-in-novel-supply-chain-attack/" target="_blank">Researcher hacks over 35 tech firms in novel supply chain attack</a>
- 패키지 매니저 프라이빗 사용하는 곳들의 레포 이름과 똑같은 이름을 퍼블릭에 배포해봤더니 악성코드가 그대로 다운로드 되었다는 글

### **npm - Catching Up with Package Lockfile Changes in v7**
<a href="https://nitayneeman.com/posts/catching-up-with-package-lockfile-changes-in-npm-v7/" target="_blank">npm - Catching Up with Package Lockfile Changes in v7</a>
- npm7 의 lockfile 이 어떻게 바꼈는지 정리한 포스트
- 더 느려지고 대신 더 안정적으로 되었다는 글

### **Capture screenshots of websites**
<a href="https://github.com/sindresorhus/capture-website" target="_blank">Capture screenshots of websites</a>
- 퍼펫티어 래핑한 웹사이트 캡쳐도구.
- 각종 셋팅을 할 수 있음
	- resolution(height, width), quality, fullpage 등
	- auth, userAgent, cookie 등

### **A markdown parser and compiler. Built for speed.**
<a href="https://github.com/markedjs/marked" target="_blank">A markdown parser and compiler. Built for speed.</a>
- marked 2.0 릴리즈

<hr>

# Javascript

### **Marko 5: eBay's UI Library Grows Up**
<a href="https://tech.ebayinc.com/engineering/ebay-launches-marko-5/" target="_blank">Marko 5: eBay's UI Library Grows Up</a>
- 이베이의 오픈 소스 JS UI 프레임웤 marko가 5버전 출시

### **Remotion: Create Videos and Motion Graphics with React**
<a href="https://www.remotion.dev/" target="_blank">Remotion: Create Videos and Motion Graphics with React</a>
- 리액트로 영상 만드는 라이브러리
- https://github.com/JonnyBurger/remotion

<hr>

## Quick Bits
### **https://devblogs.microsoft.com/typescript/announcing-typescript-4-2-rc/ 한달 전 ts 4.2 beta에 이은 rc 버전**

<hr>

## articles, opinion & tutorial

### **Sharing Data Between CSS and JavaScript with Custom Properties**
<a href="https://christianheilmann.com/2021/02/08/sharing-data-between-css-and-javascript-using-custom-properties/" target="_blank">Sharing Data Between CSS and JavaScript with Custom Properties</a>
- css variable을 조작해 js와 css간 변수 공유하는 아티클
- root.style.setProperty()를 통해 css 변수에 값을 오버라이트 하는 형태
- ```javascript
	getComputedStyle(document.documentElement).getPropertyValue('--variable')
	```

### **Accessing Hardware Devices on the Web: A Roundup of APIs**
<a href="https://web.dev/devices-introduction/" target="_blank">Accessing Hardware Devices on the Web: A Roundup of APIs</a>
- 웹에서 하드웨어 장치에 접근하는 고소준 api 모음글
- 고수준으로 충분하지 않을 때 저수준 api 사용할 것
- 키보드, 카메라, 프린터, webauth, filesystem, sensor, gps, battery, 원격재생, nfc, 블루투스 등

# Code & Tools

### **GoldenLayout: A Multi-Window Layout Manager for Webapps**
<a href="https://golden-layout.com/" target="_blank">GoldenLayout: A Multi-Window Layout Manager for Webapps</a>
- 멀티-윈도우 레이아웃 메니저인 골든 레이아웃이 2.0 릴리즈
- JQuery 디펜던시 제거하고 ts로 재작성.
- 모던 브라우저 지원

## Quick releases:

### **https://github.com/lerna/lerna/releases/tag/v4.0.0  **
모노레포 툴 lerna가 4.0 릴리즈

### **https://github.com/mochajs/mocha/releases/tag/v8.3.0**
mocha 8.3이 릴리즈

<hr>

# etc

### **https://www.youtube.com/playlist?list=PL2yQDdvlhXf9rDTxzIcc7jY8Qk1QOyl6i#reinvent2020databases**
- AWS re:invent의 모든 세션
- 해당 링크는 DB-track. 아무도 보지 않을 것 같지만 좋은게 많이 있다며 공유됨

### **https://litestream.io/blog/why-i-built-litestream/**
- boltDB 창시자가 litesteam을 만든 이유

### **https://k8s.af/**
- k8s failure stories