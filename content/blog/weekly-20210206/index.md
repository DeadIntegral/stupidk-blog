---
title: javascript weekly 2021-02-06
date: "2021-02-06T09:40:00.000Z"
description: "javascript weekly 2021-02-06"
tags: ["javascript"]
---

## Making GitHub’s New Homepage Fast and Performant
<a href="https://github.blog/2021-01-29-making-githubs-new-homepage-fast-and-performant/" target="_blank">Making GitHub’s New Homepage Fast and Performant</a>
- 깃헙 새 홈페이지 구축에 대한 5부작 아티클의 3번째
- resize, scroll 대신 IntersectionObserver 사용
- transition 명시를 통한 오염 방지
- 투명성 있는 jpg를 base64로 인코딩하고 svg로 래핑한 이미지 사용 등


## npm 7 Now Generally Available
<a href="https://github.blog/2021-02-02-npm-7-is-now-generally-available/" target="_blank">npm 7 Now Generally Available</a>
- NPM7이 디폴트 버전 적용

## The V8 v8.9 Branch
<a href="https://v8.dev/blog/v8-release-89" target="_blank">The V8 v8.9 Branch</a>
- v8 engine 8.9버전 브랜치 생성.
	- 크롬 89 버전에 top level await 적용
	- 함수의 인자 개수를 맞추지 않고 호출할 때 성능 향상
		- 언더-애플리케이션, 오버-애플리케이션
		- 아규먼트 어댑터 프레임 이라는 별도장치가 있었는데, 터보팬이 처리하도록 변경

<hr>

# Quick Bits
## https://brew.sh/2021/02/05/homebrew-3.0.0/ 홈브류 3.0 릴리즈 애플 실리콘 지원

## https://code.visualstudio.com/updates/v1_53 vscode 1월 릴리즈 다시보기

## https://aws.amazon.com/ko/blogs/mobile/amplify-javascript-releases-support-for-vue-3/ aws Amplify 에서 vue3 지원

<hr>

# Tutorials

## How JavaScript Can Now Be Executed in Oracle Database
<a href="https://medium.com/graalvm/mle-executing-javascript-in-oracle-database-c545feb1a010" target="_blank">How JavaScript Can Now Be Executed in Oracle Database</a>
- 오라클 DB c21에서 JS 지원: GraalVM
- require등 모듈 호출도 가능
	```
	DECLARE
		ctx DBMS_MLE.context_handle_t := DBMS_MLE.create_context();
		user_code clob := q'~
      const oracledb = require("mle-js-oracledb");
      const sql = "SELECT trunc(exp(4), 3) AS n FROM dual";
      // fetch NUMBER column as OracleNumber
      const options = { fetchInfo: { N: { type: oracledb.ORACLE_NUMBER } } };
      const result = oracledb.defaultConnection().execute(sql, [], options);
      // print decimal OracleNumber value
      // Output: 54.598
      console.log(result.rows[0][0].toString());
   	~';
	BEGIN
		DBMS_MLE.eval(ctx, 'JAVASCRIPT', user_code);
		DBMS_MLE.drop_context(ctx);
	END;
	```

# Code & Tools

## Vuex 4.0 Released: State Management Mechanism for Vue 3 Apps
<a href="https://next.vuex.vuejs.org/" target="_blank">Vuex 4.0 Released: State Management Mechanism for Vue 3 Apps</a>
- Vuex 4.0 릴리즈. vue3 지원.
- https://github.com/vuejs/vuex/releases/tag/v4.0.0

## v8go: Execute JavaScript from Go(lang)
<a href="https://github.com/rogchap/v8go" target="_blank">v8go: Execute JavaScript from Go(lang)</a>
- v8 context를 만들고 코드를 실행해볼 수 있는 라이브러리
- v8 dependency가 있긴하나 CI를 통한 빌드만 허용하고 직접 컴파일 안됨


## react-ultimate-resume: Your 21st Century Resume
<a href="https://github.com/welovedevs/react-ultimate-resume" target="_blank">react-ultimate-resume: Your 21st Century Resume</a>
- 온라인 이력서 작성 도구

