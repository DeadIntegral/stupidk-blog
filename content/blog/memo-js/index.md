---
title: javascript memo
date: "2020-02-03T10:00:00.000Z"
description: "javscript memo"
tags: ["javascript", "js"]
---

# tip
+ 보다 나은 조건식을 쓰는 방법 5가지  
<a href="https://scotch.io/tutorials/5-tips-to-write-better-conditionals-in-javascript" target="_blank">원문</a>
<a href="https://code-200.tistory.com/14" target="_blank">번역본</a>

+ close event detect
```javascript
window.addEventListener("beforeunload", function (event) {
	alert('정말 종료하시겠습니까?')
});
```
<a href="https://stackoverflow.com/questions/20853142/trying-to-detect-browser-close-event">stackoverflow</a>