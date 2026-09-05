---
title: "IPageSavingCallback"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "マルチページドキュメントの各ページが別々のストリームに保存されるときに呼び出されるコールバックを表します。"
type: docs
weight: 382
url: /ja/java/com.aspose.tasks/ipagesavingcallback/
---
```
public interface IPageSavingCallback
```

マルチページドキュメントの各ページが別々のストリームに保存されるときに呼び出されるコールバックを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [onFinish()](#onFinish--) | すべてのページが書き込まれたときに呼び出されるメソッドです。 |
| [pageSaving(PageSavingArgs args)](#pageSaving-com.aspose.tasks.PageSavingArgs-) | ページがストリームに保存されるときに呼び出されるメソッドです。 |
### onFinish() {#onFinish--}
```
public abstract void onFinish()
```


すべてのページが書き込まれたときに呼び出されるメソッドです。

### pageSaving(PageSavingArgs args) {#pageSaving-com.aspose.tasks.PageSavingArgs-}
```
public abstract void pageSaving(PageSavingArgs args)
```


ページがストリームに保存されるときに呼び出されるメソッドです。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| args | [PageSavingArgs](../../com.aspose.tasks/pagesavingargs) | ページ保存時の引数です。 |

