---
title: "TaskLinkDrawingCallbackDelegate"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "ガントチャートビューでタスクリンクがレンダリングされるときに呼び出されるコールバックを表します。"
type: docs
weight: 298
url: /ja/java/com.aspose.tasks/tasklinkdrawingcallbackdelegate/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.Delegate, com.aspose.ms.System.MulticastDelegate
```
public abstract class TaskLinkDrawingCallbackDelegate extends System.MulticastDelegate
```

ガントチャートビューでタスクリンクがレンダリングされるときに呼び出されるコールバックを表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [TaskLinkDrawingCallbackDelegate()](#TaskLinkDrawingCallbackDelegate--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [invoke(TaskLinkDrawingArgs args)](#invoke-com.aspose.tasks.TaskLinkDrawingArgs-) | タスクリンク描画イベントを処理するメソッドコールバックを表します。 |
### TaskLinkDrawingCallbackDelegate() {#TaskLinkDrawingCallbackDelegate--}
```
public TaskLinkDrawingCallbackDelegate()
```


### invoke(TaskLinkDrawingArgs args) {#invoke-com.aspose.tasks.TaskLinkDrawingArgs-}
```
public abstract void invoke(TaskLinkDrawingArgs args)
```


タスクリンク描画イベントを処理するメソッドコールバックを表します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| args | [TaskLinkDrawingArgs](../../com.aspose.tasks/tasklinkdrawingargs) | コールバック データを含む [TaskLinkDrawingArgs](../../com.aspose.tasks/tasklinkdrawingargs) クラスのインスタンス。 |

