---
title: "TaskTextStyleEventArgs"
second_title: "Aspose.Tasks for Java API Reference"
description: "Questa classe rappresenta un insieme di dati relativi al rendering del contenuto delle celle della tabella."
type: docs
weight: 302
url: /it/java/com.aspose.tasks/tasktextstyleeventargs/
---

**Inheritance:**
java.lang.Object
```
public class TaskTextStyleEventArgs
```

Questa classe rappresenta un insieme di dati correlati al rendering del contenuto delle celle della tabella.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getCellTextStyle()](#getCellTextStyle--) | Ottiene TextStyle che verrà utilizzato per disegnare il contenuto della cella. |
| [getColumn()](#getColumn--) | Ottiene [ViewColumn](../../com.aspose.tasks/viewcolumn) a cui appartiene la cella attualmente renderizzata. |
| [getTask()](#getTask--) | Ottiene `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) che corrisponde alla riga attualmente renderizzata. |
| [setCellTextStyle(TextStyle value)](#setCellTextStyle-com.aspose.tasks.TextStyle-) | Imposta TextStyle che verrà usato per disegnare il contenuto della cella. |
### getCellTextStyle() {#getCellTextStyle--}
```
public final TextStyle getCellTextStyle()
```


Ottiene TextStyle che verrà usato per disegnare il contenuto della cella. Questo oggetto può essere usato per personalizzare l'aspetto di una cella di tabella.

**Returns:**
[TextStyle](../../com.aspose.tasks/textstyle) - TextStyle which will be used to draw the cell's content.
### getColumn() {#getColumn--}
```
public final ViewColumn getColumn()
```


Ottiene [ViewColumn](../../com.aspose.tasks/viewcolumn) a cui appartiene la cella attualmente renderizzata.

**Returns:**
[ViewColumn](../../com.aspose.tasks/viewcolumn) - [ViewColumn](../../com.aspose.tasks/viewcolumn) to which the currently rendered cell belongs.
### getTask() {#getTask--}
```
public final Task getTask()
```


Ottiene `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) che corrisponde alla riga attualmente renderizzata.

**Returns:**
[Task](../../com.aspose.tasks/task) - `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) which corresponds to the currently rendered row.
### setCellTextStyle(TextStyle value) {#setCellTextStyle-com.aspose.tasks.TextStyle-}
```
public final void setCellTextStyle(TextStyle value)
```


Imposta TextStyle che verrà usato per disegnare il contenuto della cella. Questo oggetto può essere usato per personalizzare l'aspetto di una cella di tabella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [TextStyle](../../com.aspose.tasks/textstyle) | TextStyle che verrà usato per disegnare il contenuto della cella. |

