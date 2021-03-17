---
title: javascript weekly 2020-02-29
date: "2020-02-29T08:30:00.000Z"
description: "javascript weekly 2020-02-29"
tags: ["javascript"]
---

# V8 v8.1's Intl.DisplayNames
<a href="https://v8.dev/blog/v8-release-81" target="_blank">V8 8.1 Release</a>  
Intl.DisplayNames 이 추가되었습니다.  
languages, regions, scripts, currencies 를 번역해주는 API 입니다.  

```javascript
const zhLanguageNames = new Intl.DisplayNames(['zh-Hant'], { type: 'language' });
const enRegionNames = new Intl.DisplayNames(['en'], { type: 'region' });
const itScriptNames = new Intl.DisplayNames(['it'], { type: 'script' });
const deCurrencyNames = new Intl.DisplayNames(['de'], {type: 'currency'});

zhLanguageNames.of('fr');
// → '法文'
enRegionNames.of('US');
// → 'United States'
itScriptNames.of('Latn');
// → 'latino'
deCurrencyNames.of('JPY');
// → 'Japanischer Yen'
```

# React v16.13.0 Released
<a href="https://reactjs.org/blog/2020/02/26/react-v16.13.0.html" target="_blank">React v16.13.0 Released</a>  
+ New Warnings
	+ Warnings for some updates during render  
		다른 컴포넌트를 렌더링 하는 동안 setState를 사용하면 경고를 보여줍니다.
	+ Warnings for conflicting style rules  
		css longhand 와 shorthand 를 동시에 사용해 컨플릭트가 일어날 경우 경고를 보여줍니다.
	+ Warnings for some deprecated string refs  
		```javascript
		<Button ref="myRef" />
		```
		문자열을 참조하는 ref가 deprecated 되었습니다.


# Automated Headless Browser Scripts in Node with Puppeteer
<a href="https://www.twilio.com/blog/writing-automated-headless-browser-scripts-in-node-js-with-puppeteer" target="_blank">Puppeteer quick start</a>  
Puppeteer로 다음과 같은 기능을 순차적으로 구현해봅니다.
+ 스크린샷 찍기
+ 페이지 클릭
+ 대기 후 키보드 입력
+ 데이터 읽기  