---
title: "TaskTextStyleEventArgs"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Cette classe représente un ensemble de données liées au rendu du contenu des cellules de tableau."
type: docs
weight: 302
url: /fr/java/com.aspose.tasks/tasktextstyleeventargs/
---

**Inheritance:**
java.lang.Object
```
public class TaskTextStyleEventArgs
```

Cette classe représente un ensemble de données liées au rendu du contenu des cellules de tableau.
## Méthodes

| Méthode | Description |
| --- | --- |
| [getCellTextStyle()](#getCellTextStyle--) | Obtient TextStyle qui sera utilisé pour dessiner le contenu de la cellule. |
| [getColumn()](#getColumn--) | Obtient [ViewColumn](../../com.aspose.tasks/viewcolumn) auquel appartient la cellule actuellement rendue. |
| [getTask()](#getTask--) | Obtient `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) qui correspond à la ligne actuellement rendue. |
| [setCellTextStyle(TextStyle value)](#setCellTextStyle-com.aspose.tasks.TextStyle-) | Définit TextStyle qui sera utilisé pour dessiner le contenu de la cellule. |
### getCellTextStyle() {#getCellTextStyle--}
```
public final TextStyle getCellTextStyle()
```


Obtient TextStyle qui sera utilisé pour dessiner le contenu de la cellule. Cet objet peut être utilisé pour personnaliser l'apparence d'une cellule de tableau.

**Returns:**
[TextStyle](../../com.aspose.tasks/textstyle) - TextStyle which will be used to draw the cell's content.
### getColumn() {#getColumn--}
```
public final ViewColumn getColumn()
```


Obtient [ViewColumn](../../com.aspose.tasks/viewcolumn) auquel appartient la cellule actuellement rendue.

**Returns:**
[ViewColumn](../../com.aspose.tasks/viewcolumn) - [ViewColumn](../../com.aspose.tasks/viewcolumn) to which the currently rendered cell belongs.
### getTask() {#getTask--}
```
public final Task getTask()
```


Obtient `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) qui correspond à la ligne actuellement rendue.

**Returns:**
[Task](../../com.aspose.tasks/task) - `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) which corresponds to the currently rendered row.
### setCellTextStyle(TextStyle value) {#setCellTextStyle-com.aspose.tasks.TextStyle-}
```
public final void setCellTextStyle(TextStyle value)
```


Définit TextStyle qui sera utilisé pour dessiner le contenu de la cellule. Cet objet peut être utilisé pour personnaliser l'apparence d'une cellule de tableau.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [TextStyle](../../com.aspose.tasks/textstyle) | TextStyle qui sera utilisé pour dessiner le contenu de la cellule. |

