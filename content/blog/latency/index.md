---
title: hardware latency
date: "2020-02-10T23:00:00.000Z"
description: "모든 프로그래머가 알아야 하는 레이턴시"
tags: ["knowledge"]
---



|name|latency|
|---|---|
|L1 cache reference| 0.5 ns|
|Branch mispredict(분기 예측)| 3 ns|
|L2 cache reference| 4 ns|
|Mutex lock/unlock| 17 ns|
|Main memory reference| 100 ns|
|Compress 1KB with Zippy| 2 μs|
|Send 2KB over commodity network| 44 μs|
|SSD random read| 16 μs|
|Read 1MB sequentially form memory| 3 μs|
|Read 1MB sequentially form SSD| 49 μs|
|Read 1Mb sequentially form disk| 825 μs|
|Disk seek(디스크 검색)| 2 ms|
|Round trip in same datacenter| 500 μs|
|Send packet CA->Netherlands->CA| 150 ms|


# 용어정리
+ Branch mispredict
+ <a href="https://ko.wikipedia.org/wiki/%EC%83%81%ED%98%B8_%EB%B0%B0%EC%A0%9C">Mutex</a>
+ Disk seek