---
title: "GanttChartColumn"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Classe de vue des projets"
type: docs
weight: 111
url: /fr/java/com.aspose.tasks/ganttchartcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class GanttChartColumn extends ViewColumn
```

Classe de vue du projet
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-) | Initialise une nouvelle instance de la classe GanttChartColumn. |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-) | Initialise une nouvelle instance de la classe GanttChartColumn. |
| [GanttChartColumn(int width, int field)](#GanttChartColumn-int-int-) | Initialise une nouvelle instance de la classe GanttChartColumn. |
| [GanttChartColumn(String name, int width, int field)](#GanttChartColumn-java.lang.String-int-int-) | Initialise une nouvelle instance de la classe GanttChartColumn. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getColumnText(Task task)](#getColumnText-com.aspose.tasks.Task-) | Convertit la tâche actuelle en texte de colonne. |
| [getField()](#getField--) | Renvoie le champ de colonne. |
| [setField(int value)](#setField-int-) | Définit le champ de colonne. |
### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)
```


Initialise une nouvelle instance de la classe GanttChartColumn.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Nom de la colonne. |
| width | int | Largeur de la colonne en pixels. |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | Convertisseur de données de tâche en texte de colonne. |
| champ | int | Champ de colonne. |

### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)
```


Initialise une nouvelle instance de la classe GanttChartColumn.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Nom de la colonne. |
| width | int | Largeur de la colonne en pixels. |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | Convertisseur de données de tâche en texte de colonne. |

### GanttChartColumn(int width, int field) {#GanttChartColumn-int-int-}
```
public GanttChartColumn(int width, int field)
```


Initialise une nouvelle instance de la classe GanttChartColumn.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| width | int | Largeur de colonne en pixels. |
| champ | int | Champ de colonne. |

### GanttChartColumn(String name, int width, int field) {#GanttChartColumn-java.lang.String-int-int-}
```
public GanttChartColumn(String name, int width, int field)
```


Initialise une nouvelle instance de la classe GanttChartColumn.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Nom de la colonne. |
| width | int | Largeur de colonne en pixels. |
| champ | int | Champ de colonne. |

### getColumnText(Task task) {#getColumnText-com.aspose.tasks.Task-}
```
public final String getColumnText(Task task)
```


Convertit la tâche actuelle en texte de colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Tâche actuelle. |

**Returns:**
java.lang.String - Le texte de la colonne.
### getField() {#getField--}
```
public int getField()
```


Renvoie le champ de colonne. `Field`.

**Returns:**
int - valeur du champ de colonne.
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


Définit le champ de colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | valeur du champ de colonne. |

