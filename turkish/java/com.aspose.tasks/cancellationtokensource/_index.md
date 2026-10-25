---
title: "CancellationTokenSource"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Bir CancellationToken'a iptal edilmesi gerektiğini bildirir."
type: docs
weight: 47
url: /tr/java/com.aspose.tasks/cancellationtokensource/
---

**Inheritance:**
java.lang.Object
```
public class CancellationTokenSource
```

`CancellationToken`a iptal edilmesi gerektiğini sinyaller.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [CancellationTokenSource()](#CancellationTokenSource--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [cancel()](#cancel--) | İptal isteğini iletir. |
| [getToken()](#getToken--) | Bu `CancellationTokenSource` ile ilişkili yeni `CancellationToken`'ı oluşturur. |
| [isCancellationRequested()](#isCancellationRequested--) | Bu CancellationTokenSource için iptal isteğinin yapılıp yapılmadığını alır. |
### CancellationTokenSource() {#CancellationTokenSource--}
```
public CancellationTokenSource()
```


### cancel() {#cancel--}
```
public void cancel()
```


İptal isteğini iletir.

### getToken() {#getToken--}
```
public CancellationToken getToken()
```


Bu `CancellationTokenSource` ile ilişkili yeni `CancellationToken`'ı oluşturur.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token associated with this `CancellationTokenSource`.
### isCancellationRequested() {#isCancellationRequested--}
```
public boolean isCancellationRequested()
```


Bu CancellationTokenSource için iptal isteğinin yapılıp yapılmadığını alır.

**Returns:**
boolean - true, eğer iptal isteği yapılmışsa; aksi takdirde false.
