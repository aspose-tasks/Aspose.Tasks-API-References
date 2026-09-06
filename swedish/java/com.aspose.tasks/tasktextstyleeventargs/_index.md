---
title: "TaskTextStyleEventArgs"
second_title: "Aspose.Tasks for Java API-referens"
description: "Denna klass representerar en uppsättning data som är relaterade till rendering av tabellcellernas innehåll."
type: docs
weight: 302
url: /sv/java/com.aspose.tasks/tasktextstyleeventargs/
---

**Inheritance:**
java.lang.Object
```
public class TaskTextStyleEventArgs
```

Denna klass representerar en uppsättning data som är relaterade till rendering av en tabellcells innehåll.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getCellTextStyle()](#getCellTextStyle--) | Hämtar TextStyle som kommer att användas för att rita cellens innehåll. |
| [getColumn()](#getColumn--) | Hämtar [ViewColumn](../../com.aspose.tasks/viewcolumn) som den för närvarande renderade cellen tillhör. |
| [getTask()](#getTask--) | Hämtar `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) som motsvarar den för närvarande renderade raden. |
| [setCellTextStyle(TextStyle value)](#setCellTextStyle-com.aspose.tasks.TextStyle-) | Ställer in TextStyle som kommer att användas för att rita cellens innehåll. |
### getCellTextStyle() {#getCellTextStyle--}
```
public final TextStyle getCellTextStyle()
```


Hämtar TextStyle som kommer att användas för att rita cellens innehåll. Detta objekt kan användas för att anpassa utseendet på en tabellcell.

**Returns:**
[TextStyle](../../com.aspose.tasks/textstyle) - TextStyle which will be used to draw the cell's content.
### getColumn() {#getColumn--}
```
public final ViewColumn getColumn()
```


Hämtar [ViewColumn](../../com.aspose.tasks/viewcolumn) som den för närvarande renderade cellen tillhör.

**Returns:**
[ViewColumn](../../com.aspose.tasks/viewcolumn) - [ViewColumn](../../com.aspose.tasks/viewcolumn) to which the currently rendered cell belongs.
### getTask() {#getTask--}
```
public final Task getTask()
```


Hämtar `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) som motsvarar den för närvarande renderade raden.

**Returns:**
[Task](../../com.aspose.tasks/task) - `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) which corresponds to the currently rendered row.
### setCellTextStyle(TextStyle value) {#setCellTextStyle-com.aspose.tasks.TextStyle-}
```
public final void setCellTextStyle(TextStyle value)
```


Ställer in TextStyle som kommer att användas för att rita cellens innehåll. Detta objekt kan användas för att anpassa utseendet på en tabellcell.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [TextStyle](../../com.aspose.tasks/textstyle) | TextStyle som kommer att användas för att rita cellens innehåll. |

