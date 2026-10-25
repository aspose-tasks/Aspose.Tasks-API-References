---
title: "CancellationToken"
second_title: "Aspose.Tasks for Java API 参考"
description: "传播应取消操作的通知。"
type: docs
weight: 46
url: /zh/java/com.aspose.tasks/cancellationtoken/
---

**Inheritance:**
java.lang.Object
```
public class CancellationToken
```

传播应取消操作的通知。
## 方法

| 方法 | 描述 |
| --- | --- |
| [isCancellationRequested()](#isCancellationRequested--) | 获取此令牌是否已请求取消。 |
### isCancellationRequested() {#isCancellationRequested--}
```
public boolean isCancellationRequested()
```


获取此令牌是否已请求取消。

**Returns:**
布尔值 - 如果已请求底层 `CancellationTokenSource` 的取消则为 true；否则为 false。
