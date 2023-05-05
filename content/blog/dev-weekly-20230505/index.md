---
title: dev-weekly 2023-05-05
date: "2023-05-05T17:00:00.000Z"
description: "dev-weekly 2023-05-05"
tags: ["javascript", "css", "node", "etc"]
---
# CSS

### **[Rebuilding a featured news section with modern CSS: Vox news](https://ishadeed.com/article/rebuild-featured-news-modern-css/)**

- 뉴스기사 레이아웃 만들어보기.
- flexbox에서 order를 사용하는게 아니라, grid로 만들기, 컨테이너 쿼리를 사용한 카드 UI 등

### **[CSS Grid Gap Behavior with Hidden Elements](https://ryanmulligan.dev/blog/grid-gap)**

- `grid-template-*` 를 사용했을 때 숨김처리된 엘리먼트가 있어도 그 사이의 gap이 남는 이슈
- `grid-auto-rows`, `auto 1fr auto` 등을 활용해서 크기가 존재하는 엘리먼트 사이의 갭만 존재하게 하기

### **[CSS Only Fire](https://codepen.io/simeydotme/pen/PoyzbPM)**

- 이미지와 CSS 만으로 만든 불타는 애니메이션

# Node

### **[WebContainers now run on Safari, iOS, and iPadOS](https://blog.stackblitz.com/posts/webcontainers-are-now-supported-on-safari/)**

- WebContainer가 이제 모든 브라우저에서 지원
- 파이어폭스 베타지원, 사파리는 16.4부터 베타 지원

### **[Announcing Deno KV](https://deno.com/blog/kv)**

- 세계 35개 지역을 서포트하는 DenoKV. 지금은 waitlist에 등록해야 사용 가능
- 로컬에서 실행 관리, 아토믹 트랜잭션, 일관성 지원

### **Release**

- [chrome 113 release](https://chromereleases.googleblog.com/2023/05)
- [axios 1.4.0](https://github.com/axios/axios/releases/tag/v1.4.0)
- [marked 5.0](https://github.com/markedjs/marked/releases/tag/v5.0.0)
- [Capacitor 5.0](https://ionic.io/blog/announcing-capacitor-5)
- [msw 1.2](https://github.com/mswjs/msw/releases/tag/v1.2.1) 글 작성 시점에 1.2.1

# Javascript

### **[Angular v16 is here!](https://blog.angular.io/angular-v16-is-here-4d7a28ec680d)**

- 변경 감지 연산을 줄여 런타임 성능 향상. 시그널이 완전히 출시되면 INP가 크게 개선될 것
- 각 변경 감지 중 재계산 페널티 없이 계산된 속성 제공
- RxJS와의 더 나은 상호 운용성
- SSR, 하이드레이션 향상

### **[Badging for Home Screen Web Apps](https://webkit.org/blog/14112/badging-for-home-screen-web-apps/)**

- PWA에서 뱃지 및 알림 띄우기 예제
- 권한 확인, 알림 기능 지원 확인, 카운트 변경 등

### **[Qwik Reaches v1.0](https://www.builder.io/blog/qwik-v1)**

- JS스트리밍을 통한 즉각적인 로딩 시간
- 예측 코드 페칭 - 네트워크가 불안정한 상태에서도 사용자가 필요할 때 정확히 필요한 코드 제공
- 지연 실행 - 메인스레드를 idle상태로 유지하고 즉각적인 인터랙션 반응하도록 실행 지연
- 최적화된 렌더링 시간, 워터폴 지연을 방지하기 위한 데이터 페칭

### **[Introducing React Native macOS 0.71](https://devblogs.microsoft.com/react-native/2023-04-27-announcing-macos-71/)**

- RN MacOS 0.68 ⇒ 0.71 릴리즈. RN iOS, And, Windows와 처음으로 같은 버전
- 새로운 아키텍처 Fabric 실험적 미리 보기 제공

### **[Blur camera background](https://developer.chrome.com/en/blog/background-blur/)**

- Chrome114부터 flag 활성화를 통해 이용 가능
- 별도의 라이브러리 사용이 필요 없도록 브라우저가 지원

# ETC

### **[Writing an OS in Go: The Bootloader](https://totallygamerjet.hashnode.dev/writing-an-os-in-go-the-bootloader)**

- Go로 OS만들기 시리즈

### **[VSCode **April 2023 (version 1.78)**](https://code.visualstudio.com/updates/v1_78)**

- 터미널 버퍼 개선 - 명령어 행 사이를 키보드로 이동 가능
- 마크다운 파일에 이미지 파일 드래그하면 경로 자동 기입
- Diff 알고리즘 개선

### **[Image Carbon: 'Optimize Images, Save the Planet'](https://www.imagecarbon.com/)**

- 사이트의 주소를 입력하면 해당 사이트의 이미지들의 탄소 영향을 측정하고, 최적화 할 경우 탄소 절약의 정도를 추정해 보여주는 서비스