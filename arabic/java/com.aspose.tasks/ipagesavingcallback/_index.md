---
title: "IPageSavingCallback"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل رد نداء يتم استدعاؤه عندما يتم حفظ كل صفحة في مستند متعدد الصفحات إلى تدفق منفصل."
type: docs
weight: 382
url: /ar/java/com.aspose.tasks/ipagesavingcallback/
---
```
public interface IPageSavingCallback
```

يمثل رد نداء يتم استدعاؤه عندما يتم حفظ كل صفحة في مستند متعدد الصفحات إلى تدفق منفصل.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [onFinish()](#onFinish--) | الطريقة التي سيتم استدعاؤها عندما يتم كتابة جميع الصفحات. |
| [pageSaving(PageSavingArgs args)](#pageSaving-com.aspose.tasks.PageSavingArgs-) | الطريقة التي سيتم استدعاؤها عندما يتم حفظ صفحة إلى تدفق. |
### onFinish() {#onFinish--}
```
public abstract void onFinish()
```


الطريقة التي سيتم استدعاؤها عندما يتم كتابة جميع الصفحات.

### pageSaving(PageSavingArgs args) {#pageSaving-com.aspose.tasks.PageSavingArgs-}
```
public abstract void pageSaving(PageSavingArgs args)
```


الطريقة التي سيتم استدعاؤها عندما يتم حفظ صفحة إلى تدفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| args | [PageSavingArgs](../../com.aspose.tasks/pagesavingargs) | معاملات حفظ الصفحة. |

