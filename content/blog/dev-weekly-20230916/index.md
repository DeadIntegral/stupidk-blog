---
title: dev-weekly 2023-09-16
date: "2023-09-16T21:16:00.000Z"
description: "dev-weekly 2023-09-16"
tags: ["javascript", "node", "css"]
---

# CSS

### **[WOFF Has Left the Building](https://matthiasott.com/notes/woff-has-left-the-building)**

- caniuse에 의하면 95%의 사용자가 woff2를 지원하는 브라우저 사용. 이제 woff를 추가안해도 될 것.

### **[The new Google Fonts: find what you’re looking for](https://material.io/blog/2023-google-fonts-redesign)**

- google font 사이트는 지난 10년동안 성장하여 1500개 이상의 폰트와 6000개 이상의 머티리얼 심볼을 포함
- 사람들이 리소스를 찾는 보다 나은 방법이 필요하여 검색 추가
- 모바일 경험 향상

# Node

### **[Bun 1.0](https://bun.sh/blog/bun-v1.0)**

- 다양한 도구를 대체 - nodejs, transpiler, bundler, pakcage manager, tesing
- nextjs, remix, Nust, astro, Nest, sveltekit, solid 등의 프로젝트가 Bun에서 작동 성공
- 동일한 파일에서 esm, cjs 동시 호환
- 실험적인 Bun.exe 지원

### **[JPEG and EXIF Data Manipulation in Javascript](https://getaround.tech/exif-data-manipulation-javascript/)**

- EXIF는 이미지와 사운드의 포맷을 지정하는 표준
- JPEG 스트럭쳐의 EXIF 구조
    - 첫 4 바이트는 매직넘버. 파일 포맷 식별에 사용
    - SOI(Start of Image), …, SOS(Start of Scan), EOI(End of Image) 등 세그먼트 설명
    - JS로 세그먼트들을 이미지 버퍼에서 찾아 파싱하기
- JS로 EXIF 수정하기

### **Release**

- [fastify v4.23.0](https://github.com/fastify/fastify/releases/tag/v4.23.0)
- [electron v26.2.0](https://github.com/electron/electron/releases/tag/v26.2.0)
- [reason 3.10.0](https://github.com/reasonml/reason/releases/tag/3.10.0)
- [happy-dom v12.0.0](https://github.com/capricorn86/happy-dom/releases/tag/v12.0.0)
    - JS로 구현한 GUI 없는 웹 브라우저
- [Ant Design 5.9.0](https://github.com/ant-design/ant-design/releases/tag/5.9.0)

# Javascript

### **[Running a Playwright script on AWS Lambda](https://steele.blue/playwright-on-lambda/)**

- AWS 람다에서 playwright 실행하기 - 람다에서 설정해야 하는 이슈들
- ms에서 제공하는 의존성이 이미 설치된 도커
- `HOME=/tmp` 와 같은 컨테이너 구성 설정

### **[JavaScript WTF: Why does every() return true for empty arrays?](https://humanwhocodes.com/blog/2023/09/javascript-wtf-why-does-every-return-true-for-empty-array/)**

- JS의 `[].every(() ⇒ false)` 는 true를 반환하는 이유
- ECMA262의 구현과 수학관점(for all, exist)에서의 every

### **[JAVASCRIPT IS GETTING ARRAY GROUPING METHODS](https://philna.sh/blog/2023/09/14/javascript-array-grouping-methods/)**

- TC39 stage3에 groupBy 추가. V8에 들어갔고 FF에는 플래그로 구현. 사파리는 다른 이름으로 구현했으나 변경 예정
    
    ```jsx
    // AS-IS
    const peopleByAge = people.reduce((acc, person) => {
      const age = person.age;
      if (!acc[age]) acc[age] = [];
      acc[age].push(person);
      return acc;
    }, {});
    
    // TO-BE
    const peopleByAge = Object.groupBy(people, (person) => person.age);
    ```
    

# ETC

### **[Introducing Web Sustainability Guidelines](https://www.w3.org/blog/2023/introducing-web-sustainability-guidelines/)**

- 웹 지속 가능성 지침 소개
- 디지털 산업은 전체 탄소 배출의 2~5% 비중으로, 상위 5개 항목 중 하나
- 데이터 전송 최적화, 이미지 최적화, 친환경 호스팅 등에 대한 모범 사례와 권장 사항

### **[VSCode 1.82](https://code.visualstudio.com/updates/v1_82)**

- built-in 포트 포워딩, sticky scroll 접기/펴기
- 저장할 때 json 파일 정렬 `json.sortOnSave.enable`
- Diff Editor 강화 - 이동된 코드 UI로 표시, 변경없는 코드 접기 등
- 디버그
    - JS 디버거는 WASM 모듈을 WASM 텍스트 포맷으로 자동 디컴파일하고 중단점 설정 가능
    - 소스맵 로딩 개선
- 코파일럿 개선
    - 새 파일 생성시 인라인 채팅으로 코드 생성
    - 터미널 선택 설명
    - 설정 편집기에서 자연어 검색 지원