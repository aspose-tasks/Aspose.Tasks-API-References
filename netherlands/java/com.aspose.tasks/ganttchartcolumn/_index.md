---
title: "GanttChartColumn"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Projects view-klasse"
type: docs
weight: 111
url: /nl/java/com.aspose.tasks/ganttchartcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class GanttChartColumn extends ViewColumn
```

Projectweergaveklasse
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-) | Initialiseert een nieuw exemplaar van de GanttChartColumn-klasse. |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-) | Initialiseert een nieuw exemplaar van de GanttChartColumn-klasse. |
| [GanttChartColumn(int width, int field)](#GanttChartColumn-int-int-) | Initialiseert een nieuw exemplaar van de GanttChartColumn-klasse. |
| [GanttChartColumn(String name, int width, int field)](#GanttChartColumn-java.lang.String-int-int-) | Initialiseert een nieuw exemplaar van de GanttChartColumn-klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getColumnText(Task task)](#getColumnText-com.aspose.tasks.Task-) | Converteert de huidige taak naar de kolomtekst. |
| [getField()](#getField--) | Retourneert kolomveld. |
| [setField(int value)](#setField-int-) | Stelt kolomveld in. |
### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)
```


Initialiseert een nieuw exemplaar van de GanttChartColumn-klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | Naam van de kolom. |
| breedte | int | Breedte van de kolom in pixels. |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | Taakgegevens-naar-kolomtekst converter. |
| veld | int | Kolomveld. |

### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)
```


Initialiseert een nieuw exemplaar van de GanttChartColumn-klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | Naam van de kolom. |
| breedte | int | Breedte van de kolom in pixels. |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | Taakgegevens-naar-kolomtekst converter. |

### GanttChartColumn(int width, int field) {#GanttChartColumn-int-int-}
```
public GanttChartColumn(int width, int field)
```


Initialiseert een nieuw exemplaar van de GanttChartColumn-klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| breedte | int | Kolombreedte in pixels. |
| veld | int | Kolomveld. |

### GanttChartColumn(String name, int width, int field) {#GanttChartColumn-java.lang.String-int-int-}
```
public GanttChartColumn(String name, int width, int field)
```


Initialiseert een nieuw exemplaar van de GanttChartColumn-klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | Kolomnaam. |
| breedte | int | Kolombreedte in pixels. |
| veld | int | Kolomveld. |

### getColumnText(Task task) {#getColumnText-com.aspose.tasks.Task-}
```
public final String getColumnText(Task task)
```


Converteert de huidige taak naar de kolomtekst.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Huidige taak. |

**Returns:**
java.lang.String - De kolomtekst.
### getField() {#getField--}
```
public int getField()
```


Retourneert kolomveld. `Field`.

**Returns:**
int - kolomveldwaarde.
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


Stelt kolomveld in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | kolomveldwaarde. |

