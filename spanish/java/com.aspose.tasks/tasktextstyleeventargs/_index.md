---
title: "TaskTextStyleEventArgs"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Esta clase representa un conjunto de datos relacionados con la renderización del contenido de las celdas de la tabla."
type: docs
weight: 302
url: /es/java/com.aspose.tasks/tasktextstyleeventargs/
---

**Inheritance:**
java.lang.Object
```
public class TaskTextStyleEventArgs
```

Esta clase representa un conjunto de datos relacionados con el renderizado del contenido de la celda de tabla.
## Métodos

| Método | Descripción |
| --- | --- |
| [getCellTextStyle()](#getCellTextStyle--) | Obtiene TextStyle que se utilizará para dibujar el contenido de la celda. |
| [getColumn()](#getColumn--) | Obtiene [ViewColumn](../../com.aspose.tasks/viewcolumn) al que pertenece la celda actualmente renderizada. |
| [getTask()](#getTask--) | Obtiene `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) que corresponde a la fila actualmente renderizada. |
| [setCellTextStyle(TextStyle value)](#setCellTextStyle-com.aspose.tasks.TextStyle-) | Establece TextStyle que se usará para dibujar el contenido de la celda. |
### getCellTextStyle() {#getCellTextStyle--}
```
public final TextStyle getCellTextStyle()
```


Obtiene TextStyle que se usará para dibujar el contenido de la celda. Este objeto puede usarse para personalizar la apariencia de una celda de tabla.

**Returns:**
[TextStyle](../../com.aspose.tasks/textstyle) - TextStyle which will be used to draw the cell's content.
### getColumn() {#getColumn--}
```
public final ViewColumn getColumn()
```


Obtiene [ViewColumn](../../com.aspose.tasks/viewcolumn) al que pertenece la celda actualmente renderizada.

**Returns:**
[ViewColumn](../../com.aspose.tasks/viewcolumn) - [ViewColumn](../../com.aspose.tasks/viewcolumn) to which the currently rendered cell belongs.
### getTask() {#getTask--}
```
public final Task getTask()
```


Obtiene `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) que corresponde a la fila actualmente renderizada.

**Returns:**
[Task](../../com.aspose.tasks/task) - `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) which corresponds to the currently rendered row.
### setCellTextStyle(TextStyle value) {#setCellTextStyle-com.aspose.tasks.TextStyle-}
```
public final void setCellTextStyle(TextStyle value)
```


Establece TextStyle que se usará para dibujar el contenido de la celda. Este objeto puede usarse para personalizar la apariencia de una celda de tabla.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [TextStyle](../../com.aspose.tasks/textstyle) | TextStyle que se usará para dibujar el contenido de la celda. |

