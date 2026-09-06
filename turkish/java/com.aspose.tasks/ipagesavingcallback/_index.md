---
title: "IPageSavingCallback"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Çok sayfalı belgede her sayfa ayrı bir akışa kaydedildiğinde çağrılan bir geri aramayı temsil eder."
type: docs
weight: 382
url: /tr/java/com.aspose.tasks/ipagesavingcallback/
---
```
public interface IPageSavingCallback
```

Çok sayfalı belgede her sayfa ayrı bir akışa kaydedildiğinde çağrılan bir geri aramayı temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [onFinish()](#onFinish--) | Tüm sayfalar yazıldığında çağrılacak yöntem. |
| [pageSaving(PageSavingArgs args)](#pageSaving-com.aspose.tasks.PageSavingArgs-) | Bir sayfa bir akışa kaydedildiğinde çağrılacak yöntem. |
### onFinish() {#onFinish--}
```
public abstract void onFinish()
```


Tüm sayfalar yazıldığında çağrılacak yöntem.

### pageSaving(PageSavingArgs args) {#pageSaving-com.aspose.tasks.PageSavingArgs-}
```
public abstract void pageSaving(PageSavingArgs args)
```


Bir sayfa bir akışa kaydedildiğinde çağrılacak yöntem.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| args | [PageSavingArgs](../../com.aspose.tasks/pagesavingargs) | Sayfa kaydetme argümanları. |

