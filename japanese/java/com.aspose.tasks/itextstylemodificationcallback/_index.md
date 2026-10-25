---
title: "ITextStyleModificationCallback"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "TextStyle がテーブルセルに適用される前に呼び出されるコールバックを表します。"
type: docs
weight: 383
url: /ja/java/com.aspose.tasks/itextstylemodificationcallback/
---
```
public interface ITextStyleModificationCallback
```

TextStyle がテーブルセルに適用される前に呼び出されるコールバックを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)](#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-) | 以下のビュー（'Gantt Chart'、'Task Sheet'、'Task Usage'）でタスク行のテーブルセルをレンダリングする前に呼び出されるメソッド。 |
### beforeTaskTextStyleApplied(TaskTextStyleEventArgs args) {#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-}
```
public abstract void beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)
```


以下のビュー（'Gantt Chart'、'Task Sheet'、'Task Usage'）でタスク行のテーブルセルをレンダリングする前に呼び出されるメソッド。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| args | [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs) | この [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs) オブジェクト。 |

