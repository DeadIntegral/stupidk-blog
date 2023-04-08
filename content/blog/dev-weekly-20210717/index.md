---
title: dev-weekly 2021-07-17
date: "2021-07-17T10:30:00.000Z"
description: "dev-weekly 2021-07-17"
tags: ["javascript", "node"]
---

# Node

### **[Managing Node.js Docker Images in GitHub Packages with GitHub Actions](https://snyk.io/blog/managing-node-js-docker-images-in-github-packages-using-github-actions/)**

- 깃헙 패키지(컨테이너 레지스트리)에서 nodejs 도커 이미지 관리하는 포스트
- yml 작성 및 설명
- 레지스트리에 올라간 도커 이미지 로컬로 가져오기

### **[node.new](http://node.new)** 를 주소창에 입력하면 stackblitz 새 노트 프로젝트가 생성되어 리다이렉트

- [ts.new](http://ts.new) 를 입력하면 코드샌드박스 프론트 ts 새로운 프로젝트가 생성되어 리다이렉트(parcel)

# Javascript

### **[V8 v9.2 and the at Function](https://v8.dev/blog/v8-release-92)**

- 새로운 메서드 at - String.prototype.at, Array.prototype.at
    - [1, 2, 3].at(-1) // 3
- v8 9.2 - 공유 포인터 압축 케이지
    - 프로세스 내의 모든 격리가 동일한 4GB 가상 메모리를 공유하도록 변경

### **[Deno 1.12 Released](https://deno.com/blog/v1.12)**

- crypto api 지원
- native http 서버에서 웹소켓 지원
- repl에서 ts지원
- messageChannel, messagePort지원
- wasm 스레딩 지원 등이 있네여

### **[How to Convert Arrays to Human-Readable Lists](https://www.amitmerchant.com/how-to-convert-arrays-to-human-readable-lists-in-javascript/)**

- Intl.ListFormat

    ```jsx
    const 과일 = ['사과', '복숭아', '망고', '바나나']
    const listFormatter = new Intl.ListFormat('ko', {
        style: 'long',
        type: 'conjunction'
    })
    console.log(listFormatter.format(과일));
    // 사과, 복숭아, 망고 및 바나나
    ```

### **[The Ultimate Guide to Browser-Side Storage](https://blog.openreplay.com/the-ultimate-guide-to-browser-side-storage)**

- 변수, DOM attribute, 웹 스토리지(localStorage, sessionStorage), IndexedDB, Cache API, Cookies, File System Access API, File and Directory Entries API, window property, WebSQL 의 10가지 저장공간에 대한 설명과 예제코드 및 장던점

### **[devcert: Development SSL/TLS Certificates Made Easy](https://www.npmjs.com/package/devcert)**

- SSL/TLS 지원을 위해 자체 루트 기관을 만들고, 자동으로 인증서를 발급하도록 해주는 도구

### **[LiveKit: A Go-Powered Server for Real Time Audio and Video](https://livekit.io/)**

- realtime WebRTC 기반 오디오/비디오 경험을 구축 해주는 오픈 소스 인프라 프로젝트.
- IOS, JS, Andriod SDK 제공
- [https://livekit.io/playground](https://livekit.io/playground)