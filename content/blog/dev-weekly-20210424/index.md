---
title: dev-weekly 2021-04-24
date: "2021-04-24T09:30:00.000Z"
description: "dev-weekly 2021-04-24"
tags: ["javascript", "css", "go", "db"]
---

# CSS, Node, DB, ETC

## CSS

### **[Designing Custom Focus Indicators](https://craftcms.com/accessibility/designing-custom-focus-indicators)**

- WCAG 2.1, 2.2에서 버튼에 대한 접근성 지침이 어떻게 바뀌는지 설명한 글

---

## Node

### **[Node.js 16 Available Now](https://nodejs.medium.com/node-js-16-available-now-7f5099a97e70)**

- V8 engine 9.0으로 업데이트, 애플 실리콘 바이너리 추가, 안정적인 API
- 

    ```jsx
    import { setTimeout } from 'timers/promises';
    async function run() {
      await setTimeout(5000);
      console.log('Hello, World!');
    }
    run();
    ```

### **[Prisma ORM Toolkit Now 'Ready For Production'](https://www.prisma.io/blog/prisma-the-complete-orm-inw24qjeawmb)**

- Prisma가 할 수 있는것과 프로젝트의 방향성에 대하여

### **[Web Performance Recipes with Puppeteer](https://addyosmani.com/blog/puppeteer-recipes/)**

- 퍼펫티어를 이용해 다양한 형태의 웹 성능 지표를 얻는 방법
    - 페이지 로드에 대한 성능추적
    - 런타임 성능 메트릭
    - Lighthouse 리포트 생성, 퍼포먼스 메트릭 추출
    - 느린 네트워크와 CPU 에뮬레이션
    - JS 비활성화에서의 렌더링
    - First Paint, First Contentful Paint 측정
    - CLS(Cumulative Layout Shift) 측정
    - 메모리 누수 측정

### **[Three Services Where You Can Deploy a Node App for Free](https://blog.logrocket.com/free-services-deploy-node-js-app/)**

- 카드정보를 입력 안하고, 노드를 무료로 올릴 수 있는 서비스 3가지
- 카드정보 입력 안해도 되는곳들로여
스텝 바이 스텝 스샷넣어 가면서 굉장히 자세하게 설명해주네여

---

## DB

### **[DbGate: Another Database Desktop Client App](https://dbgate.org/)**

- 스벨트로 만들고 일렉트론입힌 크로스 플랫폼 디비 클라이언트
- MySQL, Postgres, SQL Server, MongoDB 지원

### **[Redis Labs Announces Roadmap for Redis 7.0](https://www.zdnet.com/article/redis-labs-unveils-redis-database-7-0/)**

- Redis 7.0 로드맵
- JSON 지원 - 검색(json 타입), active-active global replication.
    - [https://redislabs.com/redis-enterprise/technology/active-active-geo-distribution/](https://redislabs.com/redis-enterprise/technology/active-active-geo-distribution/)

---

## ETC

### **[0년차 아기 개발자가 15년차 개발자를 만났을 때](https://www.youtube.com/watch?v=k70Doi0JLSY)**

- 15년차 개발자가 해주는 꿀같은 조언들

---

# Javascript

### **[Solving a Mystery Behavior of parseInt()](https://dmitripavlutin.com/parseint-mystery-javascript/)**

- parseInt()에서 exponential notaion이 발생했을 때 이상현상
- ex) parseInt(0.0000005) === 5 // 5e-7이 되기 때문에

### **Quick Bits**

- [https://stackoverflow.blog/2021/04/19/how-often-do-people-actually-copy-and-paste-from-stack-overflow-now-we-know/](https://stackoverflow.blog/2021/04/19/how-often-do-people-actually-copy-and-paste-from-stack-overflow-now-we-know/)
    - 한글 요약본 [https://news.hada.io/topic?id=4120](https://news.hada.io/topic?id=4120)

## Articles, Opinions & Tutorials

### **[Five Key Lessons React Tutorials Don't Teach](https://reedbarger.hashnode.dev/5-key-lessons-react-tutorials-dont-teach)**

- setState는 비동기
- useEffect 는 도메인마다 분리해서 사용 가능
- useState, useReducer는 useCallback쓰지 않아도 되는 이유
- useRef를 통한 렌더링간의 상태유지 feat.싱글턴
- 에러 바운더리를 통한 앱 충돌 방지

## Code & Tools

### **[Sucrase: A Super-Fast Babel Alternative](https://github.com/alangpierce/sucrase)**

- 매우 빠른 바벨의 대안
- IE 서포트를 제거하여 성능을 얻은 케이스
- Jest기준으로는 바벨보다 17배 정도 빠른 성능

### **[WinBox: An HTML5 'Window Manager' for the Web](https://nextapps-de.github.io/winbox/)**

- 윈도우 스타일의 모달
- 최소화, 최대화, 전체화면 등 기능도 그대로 구현
- 하나의 페이지 안에서 수십개의 정리된 페이지 보기가 가능