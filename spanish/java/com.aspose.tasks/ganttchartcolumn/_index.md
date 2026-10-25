---
title: "GanttChartColumn"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Clase de vista de proyectos"
type: docs
weight: 111
url: /es/java/com.aspose.tasks/ganttchartcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class GanttChartColumn extends ViewColumn
```

Clase de vista del proyecto
## Constructores

| Constructor | Descripción |
| --- | --- |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-) | Inicializa una nueva instancia de la clase GanttChartColumn. |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-) | Inicializa una nueva instancia de la clase GanttChartColumn. |
| [GanttChartColumn(int width, int field)](#GanttChartColumn-int-int-) | Inicializa una nueva instancia de la clase GanttChartColumn. |
| [GanttChartColumn(String name, int width, int field)](#GanttChartColumn-java.lang.String-int-int-) | Inicializa una nueva instancia de la clase GanttChartColumn. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getColumnText(Task task)](#getColumnText-com.aspose.tasks.Task-) | Convierte la tarea actual al texto de la columna. |
| [getField()](#getField--) | Devuelve el campo de la columna. |
| [setField(int value)](#setField-int-) | Establece el campo de la columna. |
### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)
```


Inicializa una nueva instancia de la clase GanttChartColumn.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | Nombre de la columna. |
| width | int | Ancho de la columna en píxeles. |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | Convertidor de datos de tarea a texto de columna. |
| campo | int | Campo de columna. |

### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)
```


Inicializa una nueva instancia de la clase GanttChartColumn.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | Nombre de la columna. |
| width | int | Ancho de la columna en píxeles. |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | Convertidor de datos de tarea a texto de columna. |

### GanttChartColumn(int width, int field) {#GanttChartColumn-int-int-}
```
public GanttChartColumn(int width, int field)
```


Inicializa una nueva instancia de la clase GanttChartColumn.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| width | int | Ancho de columna en píxeles. |
| campo | int | Campo de columna. |

### GanttChartColumn(String name, int width, int field) {#GanttChartColumn-java.lang.String-int-int-}
```
public GanttChartColumn(String name, int width, int field)
```


Inicializa una nueva instancia de la clase GanttChartColumn.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | Nombre de la columna. |
| width | int | Ancho de columna en píxeles. |
| campo | int | Campo de columna. |

### getColumnText(Task task) {#getColumnText-com.aspose.tasks.Task-}
```
public final String getColumnText(Task task)
```


Convierte la tarea actual al texto de la columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Tarea actual. |

**Returns:**
java.lang.String - El texto de la columna.
### getField() {#getField--}
```
public int getField()
```


Devuelve el campo de la columna. `Field`.

**Returns:**
int - valor del campo de la columna.
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


Establece el campo de la columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | valor del campo de la columna. |

