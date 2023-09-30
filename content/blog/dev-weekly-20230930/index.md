---
title: dev-weekly 2023-09-30
date: "2023-09-30T11:35:00.000Z"
description: "dev-weekly 2023-09-30"
tags: ["javascript", "node", "css"]
---
# CSS

### **[Mimic.css](https://github.com/erictreacy/mimic.css)**

- css 애니메이션 라이브러리
- 졸린 눈, 떨어지는 눈물 과 같은 표현의 애니메이션

### **[Pure CSS - Holographic Death Star](https://codepen.io/maxi83c/pen/PoXJJKv)**

- HTML, CSS만으로 구현한 데스스타 홀로그램

# Node

### **[Speeding up the JavaScript ecosystem - Polyfills gone rogue](https://marvinh.dev/blog/speeding-up-javascript-ecosystem-part-6/)**

- 노드 모듈들이 큰 이유는 폴리필 때문.
- `Object.defineProperties` 는 node 0.10.0에서 제공되던 것임에도 불구하고 폴리필에 의존하는 수많은 패키지 존재.
- 폴리필은 런타임 환경에서 누락된 기능을 패치해야 하는데 직접 임포트하여 호출 중.

### **[Token based authentication with Fastify, JWT, and Typescript](https://thatarif.in/posts/token-based-authentication-with-fastify-jwt)**

- Fastify 를 사용하여 JWT 인증을 구현하는 과정
- 프로젝트 셋팅, 라우팅, 스킴작성(zod, prisma)에 이르기까지 스텝 바이 스텝 설명

# Javascript

### **[Cloudflare Fonts: enhancing website font privacy and speed](https://blog.cloudflare.com/cloudflare-fonts-enhancing-website-privacy-speed/)**

- google fonts는 html을 파싱하던 중 구글 폰트 css파일을 불러오고, 구글에는 googleapis 와 gstatic의 두 도메인이 있기 때문에 최소 4회의 네트워크 왕복이 필요
- Cloudflare fonts는 HTML이 cloudflare 네트워크를 통과할 때 재작성. 여기에는 CSS응답이 포함
- 또한 호스트 이름이나 TLS 연결 설정에 대한 추가 DNS조회가 필요하지 않음.

### **[Signal Boosting](https://preactjs.com/blog/signal-boosting/)**

- preact signal 릴리즈.
- 시그널의 동작 방식
- 과거 Set을 사용했지만 순서가 보장되지 않는 로직이 있을 수 있고, Doubly Linked list 를 선택하게 된 이유와 그 효과

### **[Tesseract.js 5.0](https://github.com/naptha/tesseract.js/releases/tag/v5.0.0)**

- 파일 사이즈 감소 (영어 54%, 중국어 73% 감소)
- 메모리 사용량 311MB → 164MB로 감소
- iOS17이 테서랙트4와의 호환성 깨뜨렸는데 5에서 이를 대응
- 브레이킹 체인지에 대해 코드 가이드 제공

### **[n64js: An Nintendo 64 emulator in JavaScript](https://github.com/hulkholden/n64js)**

- 닌텐도 64 에뮬레이터 JS버전. bun으로 컴파일

### **[JS Crush](https://js-crush.vercel.app/)**

- JS == 인 것들을 매칭시키는 게임.
- 캔디 크러시와 같은 방식.

### **Release**

- [Dependency-cruiser 14.0](https://github.com/sverweij/dependency-cruiser/releases/tag/v14.0.0)
- [Ember 5.3](https://blog.emberjs.com/ember-released-5-3/)
- [pnpm v8.8](https://github.com/pnpm/pnpm/releases/tag/v8.8.0)

# ETC

### **[Why HTTP/3 is eating the world](https://blog.apnic.net/2023/09/25/why-http-3-is-eating-the-world/)**

- HTTP3 가 나온 이유는, QUIC가 HTTP2와 호환되지 않을만큼 TCP와 다르기 때문.
- TCP의 문제점은 인터넷에 존재하는 수많은 장치가 자체적으로 TCP 프로토콜을 구현한다는 점.
    - QUIC는 TLS계층을 통합했고, 프로토콜 자체의 많은 부분도 암호화.
    - 클라이언트와 서버만 업데이트하면 됨
    - Head of line bloking 문제 해결

### **[118.0 Firefox Release](https://www.mozilla.org/en-US/firefox/118.0/releasenotes/)**

- 클라우드를 통하지 않는 웹 콘텐츠 번역 내장

### **[Your Cache Headers Could Probably be More Aggressive](https://www.macarthur.me/posts/more-aggressive-cache-headers)**

- 매번 정적 리소스를 리밸리데이트 하는 것 보다 304 응답을 하는것이 더 효과적
- vercel, netlify, cloudflare 에서 헤더 커스텀하기 예제

### **[Repo Trends: View and analyze trends in repository issues over time](https://www.repotrends.com/)**

- 레포별 시간 흐름에 따른 오픈 이슈와 풀 리퀘스트, 새 이슈와 풀 리퀘스트를 시각적으로 보여주는 서비스
- 항목에 없어도, url에 기입하면 해당 레포의 정보 출력