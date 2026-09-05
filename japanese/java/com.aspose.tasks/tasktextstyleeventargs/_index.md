---
title: "TaskTextStyleEventArgs"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "このクラスは、テーブルセルの内容のレンダリングに関連するデータの集合を表します。"
type: docs
weight: 302
url: /ja/java/com.aspose.tasks/tasktextstyleeventargs/
---

**Inheritance:**
java.lang.Object
```
public class TaskTextStyleEventArgs
```

このクラスはテーブルセルの内容のレンダリングに関連するデータのセットを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getCellTextStyle()](#getCellTextStyle--) | セルの内容を描画するために使用される TextStyle を取得します。 |
| [getColumn()](#getColumn--) | 現在レンダリングされているセルが属する [ViewColumn](../../com.aspose.tasks/viewcolumn) を取得します。 |
| [getTask()](#getTask--) | 現在レンダリングされている行に対応する `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) を取得します。 |
| [setCellTextStyle(TextStyle value)](#setCellTextStyle-com.aspose.tasks.TextStyle-) | セルの内容を描画するために使用される TextStyle を設定します。 |
### getCellTextStyle() {#getCellTextStyle--}
```
public final TextStyle getCellTextStyle()
```


セルの内容を描画するために使用される TextStyle を取得します。このオブジェクトはテーブルセルの外観をカスタマイズするために使用できます。

**Returns:**
[TextStyle](../../com.aspose.tasks/textstyle) - TextStyle which will be used to draw the cell's content.
### getColumn() {#getColumn--}
```
public final ViewColumn getColumn()
```


現在レンダリングされているセルが属する [ViewColumn](../../com.aspose.tasks/viewcolumn) を取得します。

**Returns:**
[ViewColumn](../../com.aspose.tasks/viewcolumn) - [ViewColumn](../../com.aspose.tasks/viewcolumn) to which the currently rendered cell belongs.
### getTask() {#getTask--}
```
public final Task getTask()
```


現在レンダリングされている行に対応する `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) を取得します。

**Returns:**
[Task](../../com.aspose.tasks/task) - `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) which corresponds to the currently rendered row.
### setCellTextStyle(TextStyle value) {#setCellTextStyle-com.aspose.tasks.TextStyle-}
```
public final void setCellTextStyle(TextStyle value)
```


セルの内容を描画するために使用される TextStyle を設定します。このオブジェクトはテーブルセルの外観をカスタマイズするために使用できます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [TextStyle](../../com.aspose.tasks/textstyle) | セルの内容を描画するために使用される TextStyle。 |

