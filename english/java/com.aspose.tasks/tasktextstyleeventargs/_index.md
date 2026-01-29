---
title: TaskTextStyleEventArgs
second_title: Aspose.Tasks for Java API Reference
description: This class represents set of data that related to the rendering of table cells content.
type: docs
weight: 301
url: /java/com.aspose.tasks/tasktextstyleeventargs/
---

**Inheritance:**
java.lang.Object
```
public class TaskTextStyleEventArgs
```

This class represents set of data that related to the rendering of table cell's content.
## Methods

| Method | Description |
| --- | --- |
| [getCellTextStyle()](#getCellTextStyle--) | Gets TextStyle which will be used to draw the cell's content. |
| [getColumn()](#getColumn--) | Gets [ViewColumn](../../com.aspose.tasks/viewcolumn) to which the currently rendered cell belongs. |
| [getTask()](#getTask--) | Gets `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) which corresponds to the currently rendered row. |
| [setCellTextStyle(TextStyle value)](#setCellTextStyle-com.aspose.tasks.TextStyle-) | Sets TextStyle which will be used to draw the cell's content. |
### getCellTextStyle() {#getCellTextStyle--}
```
public final TextStyle getCellTextStyle()
```


Gets TextStyle which will be used to draw the cell's content. This object can be use to customize appearance of a table cell.

**Returns:**
[TextStyle](../../com.aspose.tasks/textstyle) - TextStyle which will be used to draw the cell's content.
### getColumn() {#getColumn--}
```
public final ViewColumn getColumn()
```


Gets [ViewColumn](../../com.aspose.tasks/viewcolumn) to which the currently rendered cell belongs.

**Returns:**
[ViewColumn](../../com.aspose.tasks/viewcolumn) - [ViewColumn](../../com.aspose.tasks/viewcolumn) to which the currently rendered cell belongs.
### getTask() {#getTask--}
```
public final Task getTask()
```


Gets `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) which corresponds to the currently rendered row.

**Returns:**
[Task](../../com.aspose.tasks/task) - `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) which corresponds to the currently rendered row.
### setCellTextStyle(TextStyle value) {#setCellTextStyle-com.aspose.tasks.TextStyle-}
```
public final void setCellTextStyle(TextStyle value)
```


Sets TextStyle which will be used to draw the cell's content. This object can be use to customize appearance of a table cell.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextStyle](../../com.aspose.tasks/textstyle) | TextStyle which will be used to draw the cell's content. |

