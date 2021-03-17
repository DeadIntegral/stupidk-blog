---
title: react typescript quick-start
date: "2020-05-01T17:00:00.000Z"
description: "react typescript quick-start"
tags: ["javascript"]
---

# Setup

## use Create React App

### 새로운 프로젝트를 시작할 때
```javascript
npx create-react-app my-app --template typescript

# or

yarn create react-app my-app --template typescript
```

### 이미 존재하는 프로젝트에 TS를 추가할 때
```javascript
npm install --save typescript @types/node @types/react @types/react-dom @types/jest

# or

yarn add typescript @types/node @types/react @types/react-dom @types/jest
```
파일들의 확장자를 tsx로 변경하고, development server를 재시작해줍니다.



## not use CRA

https://createapp.dev/ 를 이용하면 쉽게 구성할 수 있습니다.


## Import React
```javascript
import * as React from "react";
```
tsconfig.json 파일에 <kbd>"allowSyntheticDefaultImports": true </kbd>를 추가하면 다음과 같이 사용할 수 있습니다.

```javascript
import React from "react";
```


# Getting Started
```javascript
type myProps = { message: string }; // interface를 사용할 수도 있습니다.
function App({message}: myProps) {
	return (<div>{message}</div>)
}
```

# 참조
https://create-react-app.dev/docs/adding-typescript/  
https://github.com/typescript-cheatsheets/react-typescript-cheatsheet  
https://createapp.dev/  



```javascript
type AppProps = {
  message: string;
  count: number;
  disabled: boolean;
  /** array of a type! */
  names: string[];
  /** string literals to specify exact string values, with a union type to join them together */
  status: "waiting" | "success";
  /** any object as long as you dont use its properties (not common) */
  obj: object;
  obj2: {}; // almost the same as `object`, exactly the same as `Object`
  /** an object with defined properties (preferred) */
  obj3: {
    id: string;
    title: string;
  };
  /** array of objects! (common) */
  objArr: {
    id: string;
    title: string;
  }[];
  /** any function as long as you don't invoke it (not recommended) */
  onSomething: Function;
  /** function that doesn't take or return anything (VERY COMMON) */
  onClick: () => void;
  /** function with named prop (VERY COMMON) */
  onChange: (id: number) => void;
  /** alternative function type syntax that takes an event (VERY COMMON) */
  onClick(event: React.MouseEvent<HTMLButtonElement>): void;
  /** an optional prop (VERY COMMON!) */
  optional?: OptionalType;
};
```

- visual hex code backtick `#000000`
- visual diff
	```diff
	- 20 test
	+ 20 test
	```
- details and summary tag. <details> details <summary>example</summary>