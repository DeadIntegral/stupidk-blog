---
title: javascript weekly 2020-04-04
date: "2020-04-04T08:30:00.000Z"
description: "javascript weekly 2020-04-04"
tags: ["javascript"]
---

#

# ES2020
<a href="https://2ality.com/2019/12/ecmascript-2020.html" target="_blank">ES2020 Final feature set</a>  
ES2020의 최종 스펙입니다. 다만, bable에서 3.8릴리즈 때 ES2020의 모든 부분을 구현했기 때문에, 이전부터 사용할 수 있었습니다.

# Typescript 3.9 beta
<a href="https://devblogs.microsoft.com/typescript/announcing-typescript-3-9-beta/" target="_blank">TypeScript 3.9 Beta Released</a>  
3.9 는 성능과 안정성에 중점을 두었고, 컴파일 타임은 약 5~10%, 머티리얼UI 가 포함된 경우 약 40%까지 빨라졌다고 합니다.

# Perflink: Low Friction JS Benchmarks You Can Share via URL
<a href="https://perf.link/" target="_blank">Perflink: Low Friction JS Benchmarks You Can Share via URL</a>  
이쁜 UI를 갖고 있으며, 로컬 저장소에 저장, 포크 저장이 가능하며, 크로스 브라우징 작동도 수행합니다.


# Rendering Charts with OffscreenCanvas
<a href="https://blog.scottlogic.com/2020/03/19/offscreen-canvas.html" target="_blank">Rendering Charts with OffscreenCanvas</a>  
오프스크린 캔버스는 캔버스 렌더링을 웹워커한테 위임시킬 수 있다고 합니다.
이는 DOM 연산이 줄어들고, 그만큼 포퍼먼스가 좋아지고요. 다만 웹워커를 바르게 사용하는 것 부터가 러닝커브가 있습니다. 그리고 여기서도 물론 RAF는 필수입니다.


# pointer-compression
<a href="https://v8.dev/blog/pointer-compression" target="_blank">A Deep Dive into Pointer Compression in V8 </a>  
2014년 크롬은 32비트에서 64비트로 넘어왔습니다. 이로인해 4바이트를 사용하던 메모리들은 8바이트를 사용하게 되었고, 크롬 팀에서는 이 4바이트의 낭비를 줄이고 싶어했습니다. 포인터 압축을 통해 어떻게 메모리 낭비를 줄였는지에 대한 포스팅입니다.


# simdjson 0.3: The Fastest JSON Parser in The World
<a href="https://lemire.me/blog/2020/03/31/we-released-simdjson-0-3-the-fastest-json-parser-in-the-world-is-even-better/" target="_blank">simdjson 0.3: The Fastest JSON Parser in The World</a>  
초당 3GB+ 를 돌파한 JSON Parser입니다. 자칭 세계에서 가장 빠르다고 하며, 충분히 빠른 하드에서는 초당 5GB도 파싱한다고 합니다.


# Node.js in a Kubernetes World
<a href="https://developer.ibm.com/articles/nodejs-kubernetes-basics/" target="_blank">Node.js in a Kubernetes World</a>  
쿠버네티스에서 노드를 사용할 때 알아야 할 7가지 입니다. 전체적인 구성을 잡아주고 설명을 해주는 글입니다만 딥 하게 설명하진 않습니다.