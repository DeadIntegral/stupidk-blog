---
title: 레디스 사용 후기
date: "2020-01-28T10:00:00.284Z"
description: "redis"
tags: ["redis"]
---

# intro

redis 란 Remote Dictionary Server  
key-value 타입의 오픈 소스 기반 DBMS로 In-memory Data Structure Store 입니다.  
1 Committer => Atomic

# install
```
sudo apt install redis-server
```

# usage
```
redis-server
```
## info
```
# 레디스의 개괄이 나옵니다.
info
```
## flush
```
# 모든 레디스의 모든 키를 삭제합니다. 매우 느립니다.
flushall

# 현재 선택된 레디스의 모든 키를 삭제합니다.
flushdb
```

# Collections
자세한 사용법은 아래 `우아한 레디스` 발표자료를 보세요!
+ String
+ List
+ Set
+ Sorted Set
+ Hash
```
Set <key> <value>
Get <key>
mset <key1> <value1> <key2> <value2> ... <keyN> <valueN>
mget <key1> <key2> ... <keyN>
hget
```

# tip & caution
+ Redis에 저장한 데이터를 읽어 올 경우 String이 됩니다.
+ 네트워크 비용이 많을 경우, lua script를 통해 api를 모방할 수 있습니다.

# performance

## best condition

## network

1Gib/s 네트워크에서 일반적인 대기 시간은 약 200 us인 반면, Unix domain socket 은 30 us 까지 빨라질 수 있습니다.
[Redis Latency](https://redis.io/topics/latency)

[우아한 Redis](https://www.slideshare.net/charsyam2/redis-196314086)
[Redis benchmark](https://redis.io/topics/benchmarks)
