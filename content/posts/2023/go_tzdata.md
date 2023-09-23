---
date: 2023-09-23
categories:
- programming
tags:
- go
title: "Time Zone 데이터베이스"
---

간혹 Go가 실행되는 환경에 time zone 데이터가 설치되지 않아서 난감한 경우가 있다.
예를 들어 AWS 특정 타입의 EC2 인스턴스나 Windows 환경인 경우 `time.LoadLocation()` 함수를 호출하면 
에러가 발생한다.
이런 경우에는 컴파일할 때 time zone 데이터베이스를 실행 바이너리에 포함시켜 주어 해결할 수 있다.

```go
package main

import (
    "fmt"
    _ "time/tzdata"
)

func main() {
    loc, err := time.LoadLocation("Pacific/Efate")
    if err != nil {
        panic(err)
    }
    fmt.Println(loc)
}
```