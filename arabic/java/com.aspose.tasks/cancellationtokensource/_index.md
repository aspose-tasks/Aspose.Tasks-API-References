---
title: "CancellationTokenSource"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يشير إلى CancellationToken أنه يجب إلغاءه."
type: docs
weight: 47
url: /ar/java/com.aspose.tasks/cancellationtokensource/
---

**Inheritance:**
java.lang.Object
```
public class CancellationTokenSource
```

يرسل إشارة إلى `CancellationToken` بأنه يجب إلغاؤه.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [CancellationTokenSource()](#CancellationTokenSource--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [cancel()](#cancel--) | ينقل طلب إلغاء. |
| [getToken()](#getToken--) | ينشئ الـ `CancellationToken` الجديد المرتبط بهذا الـ `CancellationTokenSource`. |
| [isCancellationRequested()](#isCancellationRequested--) | يحصل على ما إذا تم طلب الإلغاء لهذا CancellationTokenSource. |
### CancellationTokenSource() {#CancellationTokenSource--}
```
public CancellationTokenSource()
```


### cancel() {#cancel--}
```
public void cancel()
```


ينقل طلب إلغاء.

### getToken() {#getToken--}
```
public CancellationToken getToken()
```


ينشئ الـ `CancellationToken` الجديد المرتبط بهذا الـ `CancellationTokenSource`.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token associated with this `CancellationTokenSource`.
### isCancellationRequested() {#isCancellationRequested--}
```
public boolean isCancellationRequested()
```


يحصل على ما إذا تم طلب الإلغاء لهذا CancellationTokenSource.

**Returns:**
منطقي - true إذا تم طلب الإلغاء؛ false وإلا.
