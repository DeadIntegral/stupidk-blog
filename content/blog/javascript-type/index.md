---
title: javascript type
date: "2020-01-28T10:00:00.284Z"
description: "about javascript type"
tags: ["javascript", "type"]
---

자바스크립트의 타입은 크게 두 가지로 나뉘어집니다.  
Primitive type, Reference type 이 그것입니다.  
Primitive type에는 Number, String, Boolean, Null, Undefined, Symbol, **BingInt** 이렇게 7가지가 있습니다.

# Primitive type
## Number
`Number`는 [IEEE754 Standard](https://ko.wikipedia.org/wiki/IEEE_754)를 따릅니다.  
이는 `정수(2^53 - 1)`와 `부동소수점 숫자(64bit)`, `±0`, `±Infinite`, `NaN`을 포함합니다.  

`Number` 는 정수와 소수룰 구분하지 않고, 하나의 타입에 모두 들어갑니다.  
정수의 최대 크기는 2^53 - 1 로, 다음의 코드로 확인해볼 수 있습니다.  
```javascript
Number.MAX_SAFE_INTEGER // 9007199254740991
```
+ `NaN`은 전역 객체의 속성으로, `Not-A-Number` 를 나타냅니다.
<details>
	<summary>`NaN`은 자신을 제외한 어떤 값과 비교하더라도, 같지 않습니다.</summary>

	```javascript
	NaN === NaN // false
	NaN == NaN // false
	Number.NaN === NaN // false
	isNaN(NaN) // true
	isNaN(Number.NaN) // true
	```
	
	또한 isNaN과 Number.isNaN의 차이를 주의해야 합니다.  
	Number.isNaN은 현재 값이 NaN 일 때만 true 입니다.  
	isNaN은 현재 값 뿐만 아니라, 숫자로 변환했을 때 NaN 이면 true가 됩니다.

	```javascript
	Number.isNaN('stupidk') // false
	isNaN('stupidk') // true
	```
</details>

[MDN](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/NaN)

## String
문자열은 따옴표로 표현하는데, 3가지 표기법이 있습니다.  
```javascript
	const double = "Double Quote";
	const single = 'Single Quote';
	const back = `Back Quote - Backtick`
```
큰 따옴표와 작은 따옴표는 동치이며, 따옴표 안의 모든 내용을 텍스트로 읽습니다.
\`(backtick)은 템플릿 리터럴(Template literals) 이라고 부르며, 플레이스 홀더를 이용한 표현식을 넣을 수 있습니다. ${express}로 표기할 수 있으며, \`my name is ${age}\` 와 같이 쓸 수 있습니다.

## Boolean
`Boolean`은 `true` 와 `false` 가 있습니다.

## Null
자바스크립트의 `null`은 다른 언어와 달리 존재하지 않는, 비어있는 값을 뜻합니다.

## Undefined
## Symbol
## BigInt

[spec](https://tc39.es/ecma262/#sec-bigint-objects)
## 

# Reference type