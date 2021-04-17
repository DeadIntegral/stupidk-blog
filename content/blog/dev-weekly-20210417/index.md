---
title: dev-weekly 2021-04-17
date: "2021-04-17T10:10:00.000Z"
description: "dev-weekly 2021-04-17"
tags: ["javascript", "css", "go", "db"]
---


# CSS, Node, DB

## CSS

### [Modern CSS Upgrades To Improve Accessibility](https://moderncss.dev/modern-css-upgrades-to-improve-accessibility)

- 웹 접근성을 향상시키기 위한 CSS 팁들

### [Fig](https://github.com/withfig/autocomplete)

- VSCode 스타일 자동완성을 터미널에 추가

## Node

### [What About Bundling Yarn 1.x with Node.js? Maybe!](https://github.com/nodejs/node/pull/37277)

- 노드에 yarn 1.x 를 번들로 제공하는 이슈

### [Deno 1.9 Released](https://deno.com/blog/v1.9)

- Native HTTP/2 web server
- serde_v8 을 사용하여 오버헤드 최대 98% 절감
    - JS와 러스트 사이에서 앞뒤로 직렬화하는 대신, v8과 러스트 값 사이에서 직렬화 하여 성능 개선
- Blob URL 지원

## DB

### [Introducing OpenSearch: AWS's Fork of Elasticsearch and Kibana](https://aws.amazon.com/ko/blogs/opensource/introducing-opensearch/)

- 올해 초 엘라스틱서치와 키바나의 라이센스 변경 이슈
    - [https://www.elastic.co/kr/blog/licensing-change](https://www.elastic.co/kr/blog/licensing-change)
- 아마존에서 OpenSearch라고 하는 프로젝트로 포크
- [https://github.com/opensearch-project/OpenSearch](https://github.com/opensearch-project/OpenSearch)

### [Best practices for writing SQL queries](https://www.metabase.com/learn/building-analytics/sql-templates/sql-best-practices)

- 쿼리 작성 팁

### [SQLRite: An SQLite Clone From Scratch in Rust](https://github.com/joaoh82/rust_sqlite)

- Rust-SQLite

# JavaScript

### [Comparing the New Generation of Build Tools](https://css-tricks.com/comparing-the-new-generation-of-build-tools/)

- 모던 빌드 툴 비교
    - esbuild, snowpack, vite, wmr
    - 각 모듈의 제작자, 철학, 기본적인 사용법, 주의사항, 서포트, overall
- 하단에 요약 정리 테이블

### [Slow and Steady: Converting Sentry’s Entire Frontend to TypeScript](https://blog.sentry.io/2021/04/12/slow-and-steady-converting-sentrys-entire-frontend-to-typescript)

- 센트리가 JS 에서 TS로 컨버팅 (100%) (1100개 파일 ⇒ 1915개 파일)
- 완료할 때 까지 메이저 리팩토링 없이 진행하기로 합의 후 진행
- fowardRef는 제네릭이 되지 않아 any 로 타협

### [15 DevTool Secrets for JavaScript Developers](https://blog.asayer.io/15-devtool-secrets-for-javascript-developers)

- 크롬 개발자 도구의 편리한 기능 모음
- 크롬에 옵션을 줄 수 있음
    - -incognito - 시크릿 모드로 시작하기
    - -allow-insecure-localhost - [localhost](http://localhost) ssl 오류 무시
    - [https://peter.sh/experiments/chromium-command-line-switches/](https://peter.sh/experiments/chromium-command-line-switches/) 참조

## Code & Tools

### [Announcing react-pdf v2.0](https://react-pdf.org/blog/announcing-react-pdf-v2)

- 처음부터 새로 개발해서 v2를 제작
- 그래도 1을 호환해주나, 1은 기능 추가 중단
- svg, z-index, rgb, rgba, cmyk color, overflow, border-radius percent 등 다양한 서포트