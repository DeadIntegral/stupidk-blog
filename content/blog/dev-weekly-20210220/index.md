---
title: dev-weekly 2021-02-20
date: "2021-02-20T09:00:00.000Z"
description: "dev-weekly 2021-02-20"
tags: ["javascript", "css", "node", "web", "typescript", "go"]
---

# go, CSS, Node

### **https://blog.golang.org/go1.16**
- golang 1.16 릴리즈

### **https://snyk.io/blog/go-security-cheatsheet-for-go-developers/**
- go security cheatsheet

### **https://blog.sqreen.com/preventing-sql-injections-in-go-and-other-vulnerabilities/**
- go 에서 sql injection 방지하기

### **https://github.com/svg/svgo**
노드 기반 svg optimizer

### **https://blog.narrator.ai/generating-random-timestamps-in-sql/**
synthetic timestamp 생성하기

<hr>

### **A Table With Both a Sticky Header and a Sticky First Column**
<a href="https://css-tricks.com/a-table-with-both-a-sticky-header-and-a-sticky-first-column" target="_blank">A Table With Both a Sticky Header and a Sticky First Column</a>
- table에서 stick header, first column 을 사용하는 아티클

### **How to Create a Shrinking Header on Scroll Without JavaScript**
<a href="https://css-tricks.com/how-to-create-a-shrinking-header-on-scroll-without-javascript" target="_blank">How to Create a Shrinking Header on Scroll Without JavaScript</a>
- css 만으로 sticky 헤더의 크기를 변경하기
- viewport 바깥의 영역을 이용한 트릭

<hr>

# Javascript

### **Announcing Vite 2.0**
<a href="https://github.com/vitejs/vite" target="_blank">Announcing Vite 2.0</a>
- Vite 2.0 릴리즈
- 개발 서버에 HMR 제공
- 롤업 및 esbuild 기반 번들링과 빌드를 제공

### **V8's Super Fast super Property Access**
<a href="https://v8.dev/blog/fast-super" target="_blank">V8's Super Fast super Property Access</a>
- v8 9.0 부터는 더 빠른 super 제공

### **An Interview with Ryan Dahl, the Creator of Node.js and Deno**
<a href="https://evrone.com/ryan-dahl-interview" target="_blank">An Interview with Ryan Dahl, the Creator of Node.js and Deno</a>
- node와 deno의 창시자 라이언 달 인터뷰
- deno에 관한 이야기, 스크립트 언어, rust에 대한 이야기 등

### **V8's Route to Faster JavaScript Method Calls**
<a href="https://evrone.com/ryan-dahl-interview" target="_blank">V8's Route to Faster JavaScript Method Calls</a>
- https://v8.dev/blog/adaptor-frame
- 2월6일에 공유했던 링크(https://v8.dev/blog/v8-release-89)의 상세 내용
	- 함수의 인자 개수가 일치하지 않을 때 언어, 오버 애플리케이션
	- 아규먼트 어댑터 프레임이라는 별도 장치의 구현과 터보팬의 구현

### **Opal 1.1: A Ruby to JavaScript Compiler**
<a href="https://opalrb.com/" target="_blank">Opal 1.1: A Ruby to JavaScript Compiler</a>
- ruby to js 라이브러리 오팔이 1.1 릴리즈(https://github.com/opal/opal/releases/tag/v1.1.0)

<hr>

## Quick Bits
### **https://eyes.nasa.gov/apps/mars2020/#/home**
나사에서 threejs를 사용해 이번에 화성에 착륙한 나사 탐사선의 실시간 시뮬레이션을 렌더링

### **https://date-fns.org/docs/Getting-Started**
date-fns 문서 페이지에선 콘솔을 열고 라이브러리를 미리 사용 가능
```
init(); // init("v2.16.1" /* version */)
// _.method() 형태
_.format(new Date(2014, 1, 11), 'MM/dd/yyyy') // "02/11/2014"
```

### **https://blog.angular.io/with-best-practices-from-the-start-d64881a16de8**
앵귤러팀에서 권하는 모범사례 - 앵12 부터는 스트릭트 모드 활성화를 권장

### **https://github.com/evanw/esbuild/releases/tag/v0.8.47**
esbuild가 이제 m1 칩 지원

<hr>

## articles, opinion & tutorial

### **Learn Snowpack: A High-Performance Frontend Build Tool**
<a href="https://www.sitepoint.com/learn-snowpack/" target="_blank">Learn Snowpack: A High-Performance Frontend Build Tool</a>
- snowpack 이란 무엇인가

# Code & Tools

### **Metascraper: A Library to Scrape Metadata from Web Content**
<a href="https://metascraper.js.org/#/" target="_blank">Metascraper: A Library to Scrape Metadata from Web Content</a>
- 메타데이터 추출해주는 라이브러리

### **Neutralino 1.8: Portable, Lightweight Desktop App Framework**
<a href="https://neutralino.js.org/
" target="_blank">Neutralino 1.8: Portable, Lightweight Desktop App Framework</a>
- 앱에 크로미움 배포판 포함하는 대신 플랫폼에 내장 된 웹 뷰 컴포넌트를 사용해서 경량화

### **https://svgjar.web.app/ svg icon 모음**

## Quick releases:

<hr>

# etc