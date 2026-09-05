---
title: "CancellationTokenSource"
second_title: "Aspose.Tasks for Java API Reference"
description: "CancellationToken에 취소되어야 함을 알립니다."
type: docs
weight: 47
url: /ko/java/com.aspose.tasks/cancellationtokensource/
---

**Inheritance:**
java.lang.Object
```
public class CancellationTokenSource
```

`CancellationToken`에 취소되어야 함을 알립니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [CancellationTokenSource()](#CancellationTokenSource--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [cancel()](#cancel--) | 취소 요청을 전달합니다. |
| [getToken()](#getToken--) | 이 `CancellationTokenSource`와 연결된 새로운 `CancellationToken`을 생성합니다. |
| [isCancellationRequested()](#isCancellationRequested--) | 이 CancellationTokenSource에 대해 취소가 요청되었는지 여부를 가져옵니다. |
### CancellationTokenSource() {#CancellationTokenSource--}
```
public CancellationTokenSource()
```


### cancel() {#cancel--}
```
public void cancel()
```


취소 요청을 전달합니다.

### getToken() {#getToken--}
```
public CancellationToken getToken()
```


이 `CancellationTokenSource`와 연결된 새로운 `CancellationToken`을 생성합니다.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token associated with this `CancellationTokenSource`.
### isCancellationRequested() {#isCancellationRequested--}
```
public boolean isCancellationRequested()
```


이 CancellationTokenSource에 대해 취소가 요청되었는지 여부를 가져옵니다.

**Returns:**
boolean - 취소가 요청된 경우 true; 그렇지 않으면 false.
