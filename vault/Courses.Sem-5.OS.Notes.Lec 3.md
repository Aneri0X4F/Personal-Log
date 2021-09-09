---
id: tFy23OlAvEHgWWoRF2db5
title: OS
desc: ''
updated: 1631175550598
created: 1630900277699
stub: true
---

# System Calls and Architecture of UNIX

## Intro to system calls
* System calls are the most important and crucial concept in OS. It is basically a link connecting user to the OS.
* Formally, it is a **programming interface (like waiter connecting customers to kitchen in a restaurant)** to use the services provided by the OS. They are the programs that help give access to the functionalities provided by the OS.
*  They are written in a high-level language like C or C++.
* POSIX API is used for Linux and Win32 API is used for windows.

## Implementation of System Call
* Associated with each function call. Eg. If you call a function printf() in C, then it internally calls an associated system call telling the OS to display the written part on the scree.
* Every OS have a list of system call along with ID's.
* System call interface maintains a table with ID's as indices.
* This interface invokes a particular system call in OS kernel and returns the status and return-values if any.
* Details are hidden from programmer by the API.

## Relationship between API, System Call and OS

![](/assets/images/2021-09-09-13-13-05.png)

## Types of system calls
* File Management - Eg. create, open, close etc.
* Device Management - request, release, read, write etc.
* Protection - control access, get and set permissions etc.
* Information maintenance - get time, set process etc.
* Communications - create, delete communication, send or recieve messages etc.

### Architecture of UNIX

*![](/assets/images/%20![](/assets/images/2021-08-29-11-08-15.png).png)

* UNIX is an OS just like Linux.
* not exactly layered
* Fs is share | cc - compiler | sh - shell 
* In fact linux is based on UNIX but is more complicated than UNIX.
* UNIX system follows monolithic approach
> shell is a cmd line interface
* **In Linux or UNIX, everything is in terms of files. Thus, it becomes crucial to understand file system.**
## Few processes in shell
* date
* ps aux: gives list of all programs currently running 
* ls: list of current directories' content
* pwd - print working dir