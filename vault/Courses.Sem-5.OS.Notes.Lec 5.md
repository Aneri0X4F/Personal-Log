---
id: 2HwzsBwwTFWYs5fV9TNd9
title: Lec 1
desc: ''
updated: 1630466008642
created: 1630405589640
---

## Block suspend to block
Block suspend is waiting for event to occur in near future, and t is very high priority process, then OS will bring BS to B 

## Suspended process
* not immediately available- in sec mem
* if process in waiting condition: (the process might be block suspend state - it is independ of suspend condition - not necessary it will get executed after unblocked)
* not waiting: ready state
* possible, process itself puts itself in suspend mode when it nkows it has to wait....(recording for more)
![](/assets/images/2021-09-01-08-33-08.png)

## If process is waiting for main memory:
* State of this process - suspended process
* virtual memory - some space "considered" as main mem but not. Behaves as extended mem.
![](/assets/images/2021-09-01-08-42-00.png)