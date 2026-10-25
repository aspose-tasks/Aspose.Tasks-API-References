---
title: "CancellationTokenSource"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Memberi sinyal ke CancellationToken bahwa ia harus dibatalkan."
type: docs
weight: 47
url: /id/java/com.aspose.tasks/cancellationtokensource/
---

**Inheritance:**
java.lang.Object
```
public class CancellationTokenSource
```

Mengirim sinyal ke `CancellationToken` bahwa ia harus dibatalkan.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [CancellationTokenSource()](#CancellationTokenSource--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [cancel()](#cancel--) | Menyampaikan permintaan pembatalan. |
| [getToken()](#getToken--) | Membuat `CancellationToken` baru yang terkait dengan `CancellationTokenSource` ini. |
| [isCancellationRequested()](#isCancellationRequested--) | Mendapatkan apakah pembatalan telah diminta untuk CancellationTokenSource ini. |
### CancellationTokenSource() {#CancellationTokenSource--}
```
public CancellationTokenSource()
```


### cancel() {#cancel--}
```
public void cancel()
```


Menyampaikan permintaan pembatalan.

### getToken() {#getToken--}
```
public CancellationToken getToken()
```


Membuat `CancellationToken` baru yang terkait dengan `CancellationTokenSource` ini.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token associated with this `CancellationTokenSource`.
### isCancellationRequested() {#isCancellationRequested--}
```
public boolean isCancellationRequested()
```


Mendapatkan apakah pembatalan telah diminta untuk CancellationTokenSource ini.

**Returns:**
boolean - true, jika pembatalan telah diminta; false sebaliknya.
