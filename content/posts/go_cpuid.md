---
date: 2023-09-22
categories:
- Programming
tags:
- Go
title: "Go프로그램으로 CPU 종류와 기능 확인하기"
---

The cpuid.CPU provides access to CPU features. Use cpuid.CPU.Supports() to check for CPU features. A faster cpuid.CPU.Has() is provided which will usually be inlined by the gc compiler.

To test a larger number of features, they can be combined using f := CombineFeatures(CMOV, CMPXCHG8, X87, FXSR, MMX, SYSCALL, SSE, SSE2), etc. This can be using with cpuid.CPU.HasAll(f) to quickly test if all features are supported.

Note that for some cpu/os combinations some features will not be detected. amd64 has rather good support and should work reliably on all platforms.

Note that hypervisors may not pass through all CPU features through to the guest OS, so even if your host supports a feature it may not be visible on guests.

{{< hint info >}}
Library `https://github.com/klauspost/cpuid`: CPU feature identification for Go
{{< /hint >}}

```go
package main

import (
	"fmt"
	"strings"

	. "github.com/klauspost/cpuid/v2"
)

func main() {
	// Print basic CPU information:
	fmt.Println("Name:", CPU.BrandName)
	fmt.Println("PhysicalCores:", CPU.PhysicalCores)
	fmt.Println("ThreadsPerCore:", CPU.ThreadsPerCore)
	fmt.Println("LogicalCores:", CPU.LogicalCores)
	fmt.Println("Family", CPU.Family, "Model:", CPU.Model, "Vendor ID:", CPU.VendorID)
	fmt.Println("Features:", strings.Join(CPU.FeatureSet(), ","))
	fmt.Println("Cacheline bytes:", CPU.CacheLine)
	fmt.Println("L1 Data Cache:", CPU.Cache.L1D, "bytes")
	fmt.Println("L1 Instruction Cache:", CPU.Cache.L1I, "bytes")
	fmt.Println("L2 Cache:", CPU.Cache.L2, "bytes")
	fmt.Println("L3 Cache:", CPU.Cache.L3, "bytes")
	fmt.Println("Frequency", CPU.Hz, "hz")

	// Test if we have these specific features:
	if CPU.Supports(SSE, SSE2) {
		fmt.Println("We have Streaming SIMD 2 Extensions")
	}
}
```