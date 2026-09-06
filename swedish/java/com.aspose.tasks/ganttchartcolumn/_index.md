---
title: "GanttChartColumn"
second_title: "Aspose.Tasks for Java API-referens"
description: "Projektvy-klass"
type: docs
weight: 111
url: /sv/java/com.aspose.tasks/ganttchartcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class GanttChartColumn extends ViewColumn
```

Projektets vyklass
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-) | Initierar en ny instans av klassen GanttChartColumn. |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-) | Initierar en ny instans av klassen GanttChartColumn. |
| [GanttChartColumn(int width, int field)](#GanttChartColumn-int-int-) | Initierar en ny instans av klassen GanttChartColumn. |
| [GanttChartColumn(String name, int width, int field)](#GanttChartColumn-java.lang.String-int-int-) | Initierar en ny instans av klassen GanttChartColumn. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getColumnText(Task task)](#getColumnText-com.aspose.tasks.Task-) | Konverterar aktuell uppgift till kolumntexten. |
| [getField()](#getField--) | Returnerar kolumnfältet. |
| [setField(int value)](#setField-int-) | Ställer in kolumnfältet. |
### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)
```


Initierar en ny instans av klassen GanttChartColumn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Kolumnens namn. |
| width | int | Kolumnens bredd i pixlar. |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | Uppgiftsdata till kolumntextkonverterare. |
| fält | int | Kolumnfält. |

### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)
```


Initierar en ny instans av klassen GanttChartColumn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Kolumnens namn. |
| width | int | Kolumnens bredd i pixlar. |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | Uppgiftsdata till kolumntextkonverterare. |

### GanttChartColumn(int width, int field) {#GanttChartColumn-int-int-}
```
public GanttChartColumn(int width, int field)
```


Initierar en ny instans av klassen GanttChartColumn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| width | int | Kolumnbredd i pixlar. |
| fält | int | Kolumnfält. |

### GanttChartColumn(String name, int width, int field) {#GanttChartColumn-java.lang.String-int-int-}
```
public GanttChartColumn(String name, int width, int field)
```


Initierar en ny instans av klassen GanttChartColumn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Kolumnnamn. |
| width | int | Kolumnbredd i pixlar. |
| fält | int | Kolumnfält. |

### getColumnText(Task task) {#getColumnText-com.aspose.tasks.Task-}
```
public final String getColumnText(Task task)
```


Konverterar aktuell uppgift till kolumntexten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Aktuell uppgift. |

**Returns:**
java.lang.String - Kolumntexten.
### getField() {#getField--}
```
public int getField()
```


Returnerar kolumnfältet. `Field`.

**Returns:**
int - kolumnfältets värde.
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


Ställer in kolumnfältet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | kolumnfältets värde. |

