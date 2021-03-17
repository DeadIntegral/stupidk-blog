---
title: typescript quick start
date: "2020-03-28T20:33:00.000Z"
description: "typescript quick start for myself"
tags: ["javascript"]
---

# introduce
typescript 는 javascript superset 입니다.

## setting
타입스크립트를 설치해줍니다. 빌드에만 사용할 것이기 때문에, devDependency로 설치해도 괜찮습니다.
```
npm i -D typescript
```

프론트에서 사용할 것이기 때문에 parcel로 실행을 해줍니다. 위에서 설치를 하지 않았더라도, parcel이 필요한것들을 설치해주겠지만, parcel은 전부 dependency로 설치해줍니다. 또한 parcel이 우리가 필요로 하는 대부분의 것들을 대신 해줍니다.
```
// package.json
{
	"scripts": {
		"start": "npx parcel index.html"
	}
}
```

만약 노드를 사용한다면 tsconfig.json 파일을 만들어서 셋팅을 해줍니다.
```
{
	"compilerOptions": {
		"module": "commonjs", // export, import
		"target": "es5", // 어떤 버전으로 컴파일 할지 결정합니다.
		"sourceMap": true,
		"outDir": "./dist", // 빌드된 결과를 dist에 저장합니다.
	},
	"include": [
        "src/**/*"
	], // 포함할 파일들을 적어줍니다.
	"exclude": [
        "node_modules"
    ], // 제외할 파일들을 적어줍니다.
}
```

package.json 파일도 셋팅해줍니다.
```
"scripts": {
	"start": "node index.js",
	"prestart": "tsc",
}
```

export {} 트릭을 이용하기


js파일의 확장자만 ts로 수정하더라도 똑같이 작동합니다.
타입을 명시해줄때는 콜론(:)을 사용합니다.
```
//example
const name: string = 'stupidk';
const age: number = 30;

function printHuman(name: string, age: number): void {
	console.log(`name: ${name}, age: ${age}`)
}
```

객체를 쓸 때는 interface를 정의합니다.
```
interface Human {
	name: string,
	age: number,
	skill: Skill
}
interface Skill {
	frontend: string[],
	backend: string[],
	infra?: string[],
}

const stupidk:Human = {
	name: 'stupidk',
	age: '30',
	skill: {
		frontend: ['react', 'jquery''],
		backend: ['php', 'nodejs']
	}
}
```