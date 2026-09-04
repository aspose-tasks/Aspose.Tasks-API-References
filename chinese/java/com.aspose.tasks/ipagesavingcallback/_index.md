---
title: "IPageSavingCallback"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示一个回调，当多页文档的每一页被保存到单独的流时调用。"
type: docs
weight: 382
url: /zh/java/com.aspose.tasks/ipagesavingcallback/
---
```
public interface IPageSavingCallback
```

表示一个回调，当多页文档的每一页被保存到单独的流时调用。
## 方法

| 方法 | 描述 |
| --- | --- |
| [onFinish()](#onFinish--) | 当所有页面写入完成时将调用的方法。 |
| [pageSaving(PageSavingArgs args)](#pageSaving-com.aspose.tasks.PageSavingArgs-) | 当页面保存到流时将被调用的方法。 |
### onFinish() {#onFinish--}
```
public abstract void onFinish()
```


当所有页面写入完成时将调用的方法。

### pageSaving(PageSavingArgs args) {#pageSaving-com.aspose.tasks.PageSavingArgs-}
```
public abstract void pageSaving(PageSavingArgs args)
```


当页面保存到流时将被调用的方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| args | [PageSavingArgs](../../com.aspose.tasks/pagesavingargs) | 页面保存参数。 |

