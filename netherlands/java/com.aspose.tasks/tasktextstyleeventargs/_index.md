---
title: "TaskTextStyleEventArgs"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Deze klasse vertegenwoordigt een set gegevens die gerelateerd zijn aan het renderen van de inhoud van tabelcellen."
type: docs
weight: 302
url: /nl/java/com.aspose.tasks/tasktextstyleeventargs/
---

**Inheritance:**
java.lang.Object
```
public class TaskTextStyleEventArgs
```

Deze klasse stelt een set gegevens voor die gerelateerd zijn aan het renderen van de inhoud van een tabelcel.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getCellTextStyle()](#getCellTextStyle--) | Haalt TextStyle op die gebruikt zal worden om de inhoud van de cel te tekenen. |
| [getColumn()](#getColumn--) | Haalt [ViewColumn](../../com.aspose.tasks/viewcolumn) op waartoe de momenteel gerenderde cel behoort. |
| [getTask()](#getTask--) | Haalt `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) op die overeenkomt met de momenteel weergegeven rij. |
| [setCellTextStyle(TextStyle value)](#setCellTextStyle-com.aspose.tasks.TextStyle-) | Stelt TextStyle in die wordt gebruikt om de inhoud van de cel te tekenen. |
### getCellTextStyle() {#getCellTextStyle--}
```
public final TextStyle getCellTextStyle()
```


Haalt TextStyle op die wordt gebruikt om de inhoud van de cel te tekenen. Dit object kan worden gebruikt om het uiterlijk van een tabelcel aan te passen.

**Returns:**
[TextStyle](../../com.aspose.tasks/textstyle) - TextStyle which will be used to draw the cell's content.
### getColumn() {#getColumn--}
```
public final ViewColumn getColumn()
```


Haalt [ViewColumn](../../com.aspose.tasks/viewcolumn) op waartoe de momenteel gerenderde cel behoort.

**Returns:**
[ViewColumn](../../com.aspose.tasks/viewcolumn) - [ViewColumn](../../com.aspose.tasks/viewcolumn) to which the currently rendered cell belongs.
### getTask() {#getTask--}
```
public final Task getTask()
```


Haalt `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) op die overeenkomt met de momenteel weergegeven rij.

**Returns:**
[Task](../../com.aspose.tasks/task) - `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) which corresponds to the currently rendered row.
### setCellTextStyle(TextStyle value) {#setCellTextStyle-com.aspose.tasks.TextStyle-}
```
public final void setCellTextStyle(TextStyle value)
```


Stelt TextStyle in die wordt gebruikt om de inhoud van de cel te tekenen. Dit object kan worden gebruikt om het uiterlijk van een tabelcel aan te passen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [TextStyle](../../com.aspose.tasks/textstyle) | TextStyle die wordt gebruikt om de inhoud van de cel te tekenen. |

