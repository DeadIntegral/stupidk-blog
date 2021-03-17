---
title: javascript weekly 2020-04-11
date: "2020-04-11T08:00:00.000Z"
description: "javascript weekly 2020-04-11"
tags: ["javascript"]
---

#

# Some GitHub Pro-Tips Direct from GitHub 
<a href="https://github.blog/2020-04-09-github-protips-tips-tricks-hacks-and-secrets-from-lee-reilly/" target="_blank">Some GitHub Pro-Tips Direct from GitHub </a>  
깃헙 팁
- fuzzy path finder
- octotree
- alert new notifications
- @mention stand out
- linking code snippets
- markdown format tip
	- keyboard tag kbd <kbd>option</kbd>
	- visual hex code backtick `#000000`
	- visual diff
		```diff
		- 20 test
		+ 20 test
		```
	- details and summary tag. <details> details <summary>example</summary>
	- image center : div align="center"
	- smaller text : sup tag
- url hack : topics 뒤에 태그를 쓰고, 검색할 것을 q파라미터로 넘기기
	- ex) https://github.com/topics/minecraft?q=mod
- dark theme
- commit count
	- ex) <code>git shortlog -sn</code>, <code>git shortlog -sn --no-merges</code>

# Understanding JavaScript's Various Module Formats and Tools
<a href="https://weblogs.asp.net/dixin/understanding-all-javascript-module-formats-and-tools target="_blank">Understanding JavaScript's Various Module Formats and Tools</a>
JS 모듈에 대해 설명해줍니다.
- IIFE module: JavaScript module pattern
- Revealing module: JavaScript revealing module pattern
- CJS module: CommonJS module, or Node.js module
- AMD module: Asynchronous Module Definition, or RequireJS module
- UMD module: Universal Module Definition, or UmdJS module
- ES module: ECMAScript 2015, or ES6 module
- ES dynamic module: ECMAScript 2020, or ES11 dynamic module
- System module: SystemJS module
- Webpack module: bundle from CJS, AMD, ES modules
- Babel module: transpile from ES module
- TypeScript module: Transpile to CJS, AMD, ES, System modules
