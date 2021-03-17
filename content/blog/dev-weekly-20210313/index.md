---
title: dev-weekly 2021-03-13
date: "2021-03-13T11:30:00.000Z"
description: "dev-weekly 2021-03-13"
tags: ["javascript", "css", "node", "deno", "go"]
---

# Node, GO, DB, ETC

## Node

### [The Death of a Node.js Process](https://thomashunter.name/posts/2021-03-08-the-death-of-a-nodejs-process)

- 노드의 종료를 처리하는 방법
- process.exit(1), throw new Error(), Promise.reject(), EventEmitter#emit('error'), $ kill <PROCESS_ID>

### [Svelte NodeGUI: Build Cross Platform Apps with Node and Svelte](https://svelte.nodegui.org/)

- 스벨트로 만드는 고성능의 네이티브 플랫폼

### [Deploying a Node App to Amazon Elastic Kubernetes Service (EKS)](https://techblog.geekyants.com/amazon-eks-deploying-a-nodejs-app-using-docker-and-k8s-on-aws)

- docker, k8s, eks에 대한 개념
- 환경설정(docker, aws-cli, ecr, vpc)

### [Socket.IO 4.0.0 Released](https://socket.io/blog/socket-io-4-release/)

- 프로토콜의 변경이 없기 때문에, 이전 버전과의 통신 가능

## DB

### [Safely Reduce The Cost of Your Unused DynamoDB Tables with On-Demand Mode](https://aws.amazon.com/ko/blogs/database/safely-reduce-the-cost-of-your-unused-amazon-dynamodb-tables-using-on-demand-mode/)

- 다이나모 디비에서 온디맨드 모드를 사용해 비용절감하기

### [fsql: Search Through Your Filesystem with SQL-esque Queries](https://github.com/kashav/fsql)

- 파일 시스템에 날리는 쿼리
- go로 제작

### [Hive 2.0: A Fast Key-Value Database Written in Pure Dart](https://github.com/hivedb/hive)

- 하이브 2.0 릴리즈. 다트100%
- Stable null-safety version

## GO

### [The Go Developer Survey 2020 Results](https://blog.golang.org/survey2020-results)

- go suvery 2020 결과

### [Go Maps vs Switches](https://adayinthelifeof.nl/2021/03/04/go-map-vs-switch.html)

- go 에서 Map 과 Switch 벤치마크 비교
- O(1)인 Map이 더 느린 결과가 나옴. 어셈블리로 컴파일하여 추적

## ETC

### repl - [repl.it](http://repl.it) 에서 [https://replit.com](https://replit.com/) 로 도메인 이전

# Javascript

## Quick Bits

### [https://github.com/evanw/esbuild/releases/tag/v0.9.0](https://github.com/evanw/esbuild/releases/tag/v0.9.0)

- esbuild 0.9 릴리즈

### [https://storybook.js.org/blog/storybook-for-webpack-5/](https://storybook.js.org/blog/storybook-for-webpack-5/)

- 스토리북 웹팩5 실험적 지원

## Articles, Opinion & Tutorials

### [Going Beyond console.log() to Level Up Your Debugging Skills](https://www.sitepoint.com/beyond-console-log-level-up-your-debugging-skills/)

- live expression
- console.table($$('img:not([src^=data])'), ['src','alt'])
- 브라우저 snippet - 브라우저에 스니펫 저장하여 실행하기
- overrides 사용법 - 사이트의 코드를 내 로컬로 대체하기
- change 와 크롬에서 css 파일 수정하기

## Code & Tools

### [Taro: A Lightweight 3D Game Engine for the Web](https://github.com/Cloud9c/taro)

- threejs, connon-es 로 빌드한 가벼운 3d 게임 엔진

### [https://vole.wtf/kilobytes-gambit/](https://vole.wtf/kilobytes-gambit/) 1kb로 만들어진 체스