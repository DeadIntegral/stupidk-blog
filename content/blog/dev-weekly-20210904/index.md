---
title: dev-weekly 2021-09-04
date: "2021-09-04T16:00:00.000Z"
description: "dev-weekly 2021-09-04"
tags: ["javascript", "css", "node"]
---

# CSS, Node, etc

## CSS

### [Decoding AVIF: Deep Dive With Cats and Imgproxy](https://evilmartians.com/chronicles/decoding-avif-deep-dive-with-cats-and-imgproxy)

- 이미지에서 프레임으로
    - 최신 이미지 형식(WebP, AVIF, HEIF)은 비디오 포맷 기반
- 비디오 압축 101
    - 다운샘플링(인간의 인식 품질을 손상시키지 않으면서 크로마 채널의 디테일을 줄이고 해상도를 다운)
    - spatial locality - 각 블록을 인코딩하는 대신 이웃으로부터 예측
        - DC prediction mode
        - Directional predictions
        - AVIF에서만 사용되는 예측 모드들
- AVIF 가 정말 JPEG 보다 나은지, 어떻게 비교할 수 있는지
- imgproxy를 이용하여 이용하여 AVIF 로 변환하기 예제 feat.Docker Desktop

### [ARIA Spec for the Uninitiated: Part 1](https://www.deque.com/blog/aria-spec-for-the-uninitiated-part-1)

- ARIA의 다섯가지 규칙
    - HTML을 대신할 수 있으면 ARIA를 사용하지 않아야 합니다.
    - 네이티브 신택스를 변경하지 않습니다.
    - 모든 인터랙티브 ARIA Role은 키보드로 작동 가능해야 합니다.
    - 포커스 가능한 요소에 `role="presentation` , `aria-hidden="true"` 을 사용하지 않습니다.
    - 모든 인터랙티브 요소에는 반드시 접근 가능한 이름이 있어야 합니다.

### [CSS-Only Direction Aware Box](https://codepen.io/ainalem/full/zYwLJzG)

- 마우스가 어느 방향에서 왔는지 이펙트

## Etc

### [Ten years of Bootstrap](https://blog.getbootstrap.com/2021/08/19/ten/)

- 2021-08-19 부트스트랩 10주년
- 독스 페이지뷰 25억회, 2020년 다운로드 1.31억회
- 모든 웹사이트 중 22%에서 사용, 깃헙 프로젝트 270만개에서 사용

## Node

### [Electron 14.0.0 Released](https://www.electronjs.org/blog/electron-14-0)

- 크로미움 93, V8 9.3 적용
- 9월부터는 8주마다 릴리즈 할 예정. 9월21일 일렉트론 15출시 예정.

# Javascript

### [Visual Studio Code August 2021 Released](https://code.visualstudio.com/updates/v1_60)

- vscdoe에 붙여넣기 할 때 언어 감지
- 커스텀 터미널 글리프 렌더링
- 에디터 그룹 락

### [Neutralino 2.7: Portable, Lightweight Desktop App Framework](https://neutralino.js.org/)

- 일렉트론이나 NWjs와 달리 의존성 라이브러리를 설치하지 않음
- os의 기존 웹 브라우저 라이브러리를 사용

### [interactive learning tools](https://www.smashingmagazine.com/2021/09/interactive-learning-tools-front-end-developers/)

- 게임과 같은 인터랙티브하게 학습하는 서비스 모음
- CSS, React, JS, Design Pattern, Service Worker, SQL, Vim, Jamstack

### [Twitter's div Soup and Uglyfied CSS, Explained](https://giuseppegurgone.com/twitter-html/)

- RN for Web으로 만들어진 트위터 코드 분석

### [Relay 12.0](https://github.com/facebook/relay/releases/tag/v12.0.0)

- 릴레이 12.0 릴리즈

### [Common npm Mistakes Every Developer Should Avoid](https://blog.bitsrc.io/common-npm-mistakes-every-developer-should-avoid-60ab0642d8f9)

- NPM 을 사용하면서 피해야할 실수 7가지

### [State Management in Svelte Apps](https://auth0.com/blog/state-management-in-svelte-applications/)

- 스벨트에서 상태관리하기

### [Stitches 1.0: The Modern Styling Library](https://stitches.dev/)

- 스티치 1.0 릴리즈

### [bundle: A Quick npm Package Size Checker](https://bundle.js.org/)

- 패키지를 넣으면 번들 사이즈를 제공해줍니다.