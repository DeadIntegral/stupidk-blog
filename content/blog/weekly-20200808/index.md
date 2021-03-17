---
title: javascript weekly 2020-08-08
date: "2020-08-08T09:30:00.000Z"
description: "javascript weekly 2020-08-08"
tags: ["javascript"]
---

# 1Keys: How I Made a Piano in Only 1KB of JavaScript
<a href="https://frankforce.com/?p=7617#pianostory" target="_blank">1Keys: How I Made a Piano in Only 1KB of JavaScript</a>
- JS1024 우승작. 피아노라고 하지만, 다양한 악기의 연주 가능
- 키도 맵핑하여 키보드로 연주 가능한 프로젝트
- 결과확인 - https://js1024.fun/results/2020

# Announcing the New TypeScript Website
<a href="https://devblogs.microsoft.com/typescript/announcing-the-new-typescript-website/" target="_blank">Announcing the New TypeScript Website</a>
- 오피셜 TS사이트 개선
- docs, handbook, playground 등 다양한 서비스
- playground에서는 dts 추출, npm 설치 등 다양한 기능 제공
- https://www.typescriptlang.org/


# A Roadmap for the Future of Angular
<a href="https://blog.angular.io/a-roadmap-for-angular-1b4fa996a771" target="_blank">A Roadmap for the Future of Angular</a>
- 오피셜 앵귤러 사이트 개선
- 로드맵 제공 https://angular.io/guide/roadmap

<hr>

# 3 Common Mistakes When Using Promises
<a href="https://dev.to/mpodlasin/3-most-common-mistakes-when-using-promises-in-javascript-oab" target="_blank">3 Common Mistakes When Using Promises</a>
- promise를 사용할 때 자주하는 실수 3가지
- 1. promise 중첩 할 필요 없다.
```
// bed
const createdPromise = new Promise(resolve => {
  somePreviousPromise.then(result => {
    // do something with the result
    resolve(result);
  });
});
// good
const createdPromise = somePreviousPromise.then(result => {
  // do something with result
  return result;
});
```

# Matching Accented Letters in Regular Expressions
<a href="https://davidwalsh.name/regex-accented-letters" target="_blank">Matching Accented Letters in Regular Expressions</a>
- 정규식에서 A-z 로 필터를 걸면 악센트 있는 문자는 캐칭이 안됨
```
// Single word
"Özil".match(/[\p{Letter}]+/gu)

// Word with spaces
"Oğuzhan Özyakup".match(/[\p{Letter}\s]+/gu);
```