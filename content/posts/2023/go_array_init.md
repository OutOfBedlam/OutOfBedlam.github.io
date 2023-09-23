---
date: 2023-09-23
categories:
- programming
tags:
- go
title: "Go 배열/슬라이스 초기화"
---

TIL;

- 미리 정의된 값을 사용하여 배열을 초기화 할 때 배열을 길이를 지정하지 않고 `[...]type`을 사용할 수 있다. 컴파일러가 지정된 값에 따라 알아서 해준다.
- 배열과 슬라이스를 초기화 할 때 각 값마다 `index:value` 형태로 인덱스 위치를 지정할 수 있다. 

> https://github.com/golang/go/blob/master/src/syscall/zerrors_linux_arm.go
> 

```go
var errors = [...]string{
	1:   "operation not permitted",
	2:   "no such file or directory",
	3:   "no such process",
	4:   "interrupted system call",
	5:   "input/output error",
    // 생략
    131: "state not recoverable",
	132: "operation not possible due to RF-kill",
	133: "unknown error 133",
}
```