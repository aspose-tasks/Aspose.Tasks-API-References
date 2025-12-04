---
title: IPageSavingCallback
second_title: Aspose.Tasks for Java API Reference
description: Represents a callback that is called when each page in multi page document is saved to a separate stream.
type: docs
weight: 379
url: /java/com.aspose.tasks/ipagesavingcallback/
---
```
public interface IPageSavingCallback
```

Represents a callback that is called when each page in multi page document is saved to a separate stream.
## Methods

| Method | Description |
| --- | --- |
| [onFinish()](#onFinish--) | Method which will be called when all pages are written. |
| [pageSaving(PageSavingArgs args)](#pageSaving-com.aspose.tasks.PageSavingArgs-) | The method to be called when a page is saved to a stream. |
### onFinish() {#onFinish--}
```
public abstract void onFinish()
```


Method which will be called when all pages are written.

### pageSaving(PageSavingArgs args) {#pageSaving-com.aspose.tasks.PageSavingArgs-}
```
public abstract void pageSaving(PageSavingArgs args)
```


The method to be called when a page is saved to a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| args | [PageSavingArgs](../../com.aspose.tasks/pagesavingargs) | The page saving arguments. |

