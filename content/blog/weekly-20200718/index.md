---
title: javascript weekly 2020-07-18
date: "2020-07-18T09:30:00.000Z"
description: "javascript weekly 2020-07-18"
tags: ["javascript"]
---

# Super Expressive: Build Regexes in (Almost) Natural Language
<a href="https://github.com/francisrstokes/super-expressive" target="_blank">Super Expressive: Build Regexes in (Almost) Natural Language</a>
- 자연어와 같은 형태로 코드를 전개하면, 정규식으로 만들어주는 라이브러리
```javascript
const SuperExpressive = require('super-expressive');

const myRegex = SuperExpressive()
  .startOfInput
  .optional.string('0x')
  .capture
    .exactly(4).anyOf
      .range('A', 'F')
      .range('a', 'f')
      .range('0', '9')
    .end()
  .end()
  .endOfInput
  .toRegex();

// Produces the following regular expression:
/^(?:0x)?([A-Fa-f0-9]{4})$/
```

# Apollo Client 3.0 Released: The Full Featured GraphQL Client 
<a href="https://www.apollographql.com/blog/announcing-the-release-of-apollo-client-3-0/" target="_blank">Apollo Client 3.0 Released: The Full Featured GraphQL Client </a>
- A single, consolidated @apollo/client package
- New InMemoryCache APIs
- Improved local state management
- Expanded and refined UI reactivity
- Extensive internal refactoring

<hr>

# Quick bytes
## https://github.com/hapijs/hapi/issues/4113 스폰서쉽이후 hapi의 부활

<hr>

# Generating UUIDs at Scale on the Web
<a href="https://medium.com/teads-engineering/generating-uuids-at-scale-on-the-web-2877f529d2a2" target="_blank">Generating UUIDs at Scale on the Web</a>
- uuid란 무엇인가
- 웹 브라우저에서 uuid4 사용후기


# Code & Tools
## React Native 0.63 Released
<a href="https://reactnative.dev/blog/2020/07/06/version-0.63" target="_blank">React Native 0.63 Released</a>
- 리액트 네이티브 0.63 릴리즈

## dequal: A Tiny (305B) Utility for Check for Deep Equality
<a href="https://github.com/lukeed/dequal" target="_blank">dequal: A Tiny (305B) Utility for Check for Deep Equality</a>
- 작고 매우 빠른 깊은 비교