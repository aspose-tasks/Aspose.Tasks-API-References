---
title: "IPageSavingCallback"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili callback yang dipanggil ketika setiap halaman dalam dokumen multi halaman disimpan ke aliran terpisah."
type: docs
weight: 382
url: /id/java/com.aspose.tasks/ipagesavingcallback/
---
```
public interface IPageSavingCallback
```

Mewakili callback yang dipanggil ketika setiap halaman dalam dokumen multi halaman disimpan ke aliran terpisah.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [onFinish()](#onFinish--) | Metode yang akan dipanggil ketika semua halaman telah ditulis. |
| [pageSaving(PageSavingArgs args)](#pageSaving-com.aspose.tasks.PageSavingArgs-) | Metode yang akan dipanggil ketika sebuah halaman disimpan ke aliran. |
### onFinish() {#onFinish--}
```
public abstract void onFinish()
```


Metode yang akan dipanggil ketika semua halaman telah ditulis.

### pageSaving(PageSavingArgs args) {#pageSaving-com.aspose.tasks.PageSavingArgs-}
```
public abstract void pageSaving(PageSavingArgs args)
```


Metode yang akan dipanggil ketika sebuah halaman disimpan ke aliran.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| args | [PageSavingArgs](../../com.aspose.tasks/pagesavingargs) | Argumen penyimpanan halaman. |

