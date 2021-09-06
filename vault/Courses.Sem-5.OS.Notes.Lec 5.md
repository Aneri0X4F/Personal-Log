---
id: 2HwzsBwwTFWYs5fV9TNd9
title: Lec 1
desc: ''
updated: 1630467868339
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

## PCB
* process control block
* Process identification: 
    * unique identifier for each process by process id
    * same for its parent by maintaining its parent id and user id
    * total 3 id
## Processor state information
* Control and status registers
    * Program counter: address of next instruction to be fetched
    * condition codes
    * status info : enabled/ idsabled falgs
* stack pointer
* process control information
    * process state(running/ready/blocked): scheduling a state info
    * inter process communication IPC
    * process privilages
