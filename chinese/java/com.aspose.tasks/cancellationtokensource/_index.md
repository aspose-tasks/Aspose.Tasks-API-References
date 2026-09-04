---
title: "CancellationTokenSource"
second_title: "Aspose.Tasks for Java API 参考"
description: "向 CancellationToken 发出应取消的信号。"
type: docs
weight: 47
url: /zh/java/com.aspose.tasks/cancellationtokensource/
---

**Inheritance:**
java.lang.Object
```
public class CancellationTokenSource
```

向 `CancellationToken` 发出应取消的信号。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [CancellationTokenSource()](#CancellationTokenSource--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [cancel()](#cancel--) | 传达取消请求。 |
| [getToken()](#getToken--) | 创建与此 `CancellationTokenSource` 关联的新 `CancellationToken`。 |
| [isCancellationRequested()](#isCancellationRequested--) | 获取此 CancellationTokenSource 是否已请求取消。 |
### CancellationTokenSource() {#CancellationTokenSource--}
```
public CancellationTokenSource()
```


### cancel() {#cancel--}
```
public void cancel()
```


传达取消请求。

### getToken() {#getToken--}
```
public CancellationToken getToken()
```


创建与此 `CancellationTokenSource` 关联的新 `CancellationToken`。

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token associated with this `CancellationTokenSource`.
### isCancellationRequested() {#isCancellationRequested--}
```
public boolean isCancellationRequested()
```


获取此 CancellationTokenSource 是否已请求取消。

**Returns:**
boolean - true，如果已请求取消；false，否则。
