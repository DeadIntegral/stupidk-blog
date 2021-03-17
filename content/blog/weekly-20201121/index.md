---
title: javascript weekly 2020-11-21
date: "2020-11-21T09:30:00.000Z"
description: "javascript weekly 2020-11-21"
tags: ["javascript"]
---

## TypeScript 4.1 Released
<a href="https://devblogs.microsoft.com/typescript/announcing-typescript-4-1/" target="_blank">TypeScript 4.1 Released</a>
- Template Literal Types
	- 타입 선언을 템플릿 리터럴처럼 사용할 수 있게 해줍니다.
	```javascript
	type Color = "red" | "blue";
	type Quantity = "one" | "two";
  
	type SeussFish = `${Quantity | Color} fish`;
	// same as
	//   type SeussFish = "one fish" | "two fish"
	//                  | "red fish" | "blue fish";
	```
- Key Remapping in Mapped Types
- Recursive Conditional Types
- Checked Indexed Accesses
- paths without baseUrl
- checkJs Implies allowJs
- React 17 JSX Factories
- Editor Support for the JSDoc @see Tag
- Conditional Spreads Create Optional Properties

## A Tale of Going from JavaScript to WebAssembly
<a href="https://engineering.q42.nl/webassembly/" target="_blank">A Tale of Going from JavaScript to WebAssembly</a>
- WASM으로 마이그레이션한 포스트
- EMSCription
- AssemblyScript
- AssemblyScript + WebGL
- IE에 대한 폴리필

## Prettier 2.2 Released
<a href="https://prettier.io/blog/2020/11/20/2.2.0.html" target="_blank">Prettier 2.2 Released</a>
- 새로운 JS 파서 espree(ESLint 파서) 와 meriyah 지원
	- https://github.com/eslint/espree
	- https://github.com/meriyah/meriyah
- TS 4.1 지원
- 최신 브라우저용 ESM 스탠드얼론 번들 제공

## Electron 11 Released with Experimental Apple Silicon Support
<a href="https://www.electronjs.org/releases/stable#11.0.0" target="_blank">Electron 11 Released with Experimental Apple Silicon Support</a>
- 크롬87 종속성 업데이트
- new experimental apple silicon

<hr>

# Tutorials

## https://snyk.io/blog/10-react-security-best-practices/ 리액트 보안사항

## A Super Simple Start to Firebase Functions
<a href="https://kentcdodds.com/blog/super-simple-start-to-firebase-functions" target="_blank">A Super Simple Start to Firebase Functions</a>
- 파이어 베이스를 사용하여 서버 구축하기

# Code & Tools

## jose: Universal 'JSON Web Almost Everything'
<a href="https://github.com/panva/jose" target="_blank">jose: Universal 'JSON Web Almost Everything'</a>
- JSON Web 이 너무 많기 때문에 유니버설 제작
- JWA, JWS, JWE, JWT, JWK 등
