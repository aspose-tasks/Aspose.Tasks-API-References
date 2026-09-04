---
title: "TaskTextStyleEventArgs"
second_title: "Aspose.Tasks for Java API 参考"
description: "此类表示与表格单元格内容渲染相关的数据集合。"
type: docs
weight: 302
url: /zh/java/com.aspose.tasks/tasktextstyleeventargs/
---

**Inheritance:**
java.lang.Object
```
public class TaskTextStyleEventArgs
```

此类表示与表格单元格内容渲染相关的数据集。
## 方法

| 方法 | 描述 |
| --- | --- |
| [getCellTextStyle()](#getCellTextStyle--) | 获取用于绘制单元格内容的 TextStyle。 |
| [getColumn()](#getColumn--) | 获取当前渲染的单元格所属的 [ViewColumn](../../com.aspose.tasks/viewcolumn)。 |
| [getTask()](#getTask--) | 获取对应当前渲染行的 `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-))。 |
| [setCellTextStyle(TextStyle value)](#setCellTextStyle-com.aspose.tasks.TextStyle-) | 设置用于绘制单元格内容的 TextStyle。 |
### getCellTextStyle() {#getCellTextStyle--}
```
public final TextStyle getCellTextStyle()
```


获取用于绘制单元格内容的 TextStyle。此对象可用于自定义表格单元格的外观。

**Returns:**
[TextStyle](../../com.aspose.tasks/textstyle) - TextStyle which will be used to draw the cell's content.
### getColumn() {#getColumn--}
```
public final ViewColumn getColumn()
```


获取当前渲染的单元格所属的 [ViewColumn](../../com.aspose.tasks/viewcolumn)。

**Returns:**
[ViewColumn](../../com.aspose.tasks/viewcolumn) - [ViewColumn](../../com.aspose.tasks/viewcolumn) to which the currently rendered cell belongs.
### getTask() {#getTask--}
```
public final Task getTask()
```


获取对应当前渲染行的 `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-))。

**Returns:**
[Task](../../com.aspose.tasks/task) - `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) which corresponds to the currently rendered row.
### setCellTextStyle(TextStyle value) {#setCellTextStyle-com.aspose.tasks.TextStyle-}
```
public final void setCellTextStyle(TextStyle value)
```


设置用于绘制单元格内容的 TextStyle。此对象可用于自定义表格单元格的外观。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [TextStyle](../../com.aspose.tasks/textstyle) | 用于绘制单元格内容的 TextStyle。 |

