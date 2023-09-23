---
date: 2023-09-23
categories:
- macos
title: macOS 자동 실행 프로그램들
---


자동으로 실행되는 백그라운드 프로세스들 중 애플에서 배포된 것이 아닌 것들을 확인하는 방법.

```bash
launchctl list | grep -v "com.apple"
```

자동 실행되는 프로세스를 제거하는 방법.

```bash
launchctl remove com.google.keystone.system.agent
```