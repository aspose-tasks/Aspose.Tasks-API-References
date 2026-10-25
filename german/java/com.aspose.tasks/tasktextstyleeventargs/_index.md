---
title: "TaskTextStyleEventArgs"
second_title: "Aspose.Tasks for Java API Reference"
description: "Diese Klasse repräsentiert eine Menge von Daten, die mit der Darstellung des Inhalts von Tabellenzellen zusammenhängen."
type: docs
weight: 302
url: /de/java/com.aspose.tasks/tasktextstyleeventargs/
---

**Inheritance:**
java.lang.Object
```
public class TaskTextStyleEventArgs
```

Diese Klasse stellt einen Datensatz dar, der sich auf das Rendern des Inhalts von Tabellenzellen bezieht.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getCellTextStyle()](#getCellTextStyle--) | Ruft TextStyle ab, das zum Zeichnen des Zellinhalts verwendet wird. |
| [getColumn()](#getColumn--) | Ruft [ViewColumn](../../com.aspose.tasks/viewcolumn) ab, zu dem die aktuell gerenderte Zelle gehört. |
| [getTask()](#getTask--) | Ruft `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) ab, das der aktuell gerenderten Zeile entspricht. |
| [setCellTextStyle(TextStyle value)](#setCellTextStyle-com.aspose.tasks.TextStyle-) | Setzt TextStyle, das zum Zeichnen des Zellinhalts verwendet wird. |
### getCellTextStyle() {#getCellTextStyle--}
```
public final TextStyle getCellTextStyle()
```


Ruft TextStyle ab, das zum Zeichnen des Zellinhalts verwendet wird. Dieses Objekt kann verwendet werden, um das Aussehen einer Tabellenzelle anzupassen.

**Returns:**
[TextStyle](../../com.aspose.tasks/textstyle) - TextStyle which will be used to draw the cell's content.
### getColumn() {#getColumn--}
```
public final ViewColumn getColumn()
```


Ruft [ViewColumn](../../com.aspose.tasks/viewcolumn) ab, zu dem die aktuell gerenderte Zelle gehört.

**Returns:**
[ViewColumn](../../com.aspose.tasks/viewcolumn) - [ViewColumn](../../com.aspose.tasks/viewcolumn) to which the currently rendered cell belongs.
### getTask() {#getTask--}
```
public final Task getTask()
```


Ruft `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) ab, das der aktuell gerenderten Zeile entspricht.

**Returns:**
[Task](../../com.aspose.tasks/task) - `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) which corresponds to the currently rendered row.
### setCellTextStyle(TextStyle value) {#setCellTextStyle-com.aspose.tasks.TextStyle-}
```
public final void setCellTextStyle(TextStyle value)
```


Setzt TextStyle, das zum Zeichnen des Zellinhalts verwendet wird. Dieses Objekt kann verwendet werden, um das Aussehen einer Tabellenzelle anzupassen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [TextStyle](../../com.aspose.tasks/textstyle) | TextStyle, das zum Zeichnen des Zellinhalts verwendet wird. |

