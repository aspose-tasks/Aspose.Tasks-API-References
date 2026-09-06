---
title: "ProjectView"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Clase de vista de proyectos"
type: docs
weight: 228
url: /es/java/com.aspose.tasks/projectview/
---

**Inheritance:**
java.lang.Object
```
public class ProjectView
```

Clase de vista del proyecto
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ProjectView(Iterable&lt;ViewColumn&gt; columns)](#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--) | Inicializa una nueva instancia de la clase [ProjectView](../../com.aspose.tasks/projectview). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getColumns()](#getColumns--) | Obtiene las columnas de la vista del proyecto. |
| [getDefaultAssignmentView()](#getDefaultAssignmentView--) | Incluye columnas Uid, nombre de tarea, nombre de recurso, trabajo y duración de asignación. |
| [getDefaultGanttChartView()](#getDefaultGanttChartView--) | Incluye columnas de tarea id, indicadores, nombre, duración, inicio y fin. |
| [getDefaultResourceSheetView()](#getDefaultResourceSheetView--) | Incluye columnas de recurso Uid, nombre del recurso, tipo, etiqueta de material, iniciales, grupo, unidades máximas, tarifa estándar, tarifa de horas extra, costo por uso, acumulado en, calendario base y código de recurso. |
| [getDefaultResourceUsageView()](#getDefaultResourceUsageView--) | Incluye columnas de recurso de trabajo uid, nombre, inicio, fin y trabajo. |
| [getDefaultTaskSheetView()](#getDefaultTaskSheetView--) | Incluye columnas de tarea id, indicadores, nombre, duración, inicio, fin, predecesores y nombres de recursos. |
### ProjectView(Iterable&lt;ViewColumn&gt; columns) {#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--}
```
public ProjectView(Iterable<ViewColumn> columns)
```


Inicializa una nueva instancia de la clase [ProjectView](../../com.aspose.tasks/projectview).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnas | java.lang.Iterable&lt;com.aspose.tasks.ViewColumn&gt; | Una lista de las columnas de vista. |

### getColumns() {#getColumns--}
```
public final List<ViewColumn> getColumns()
```


Obtiene las columnas de la vista del proyecto.

**Returns:**
java.util.List&lt;com.aspose.tasks.ViewColumn&gt; - las columnas de vista del proyecto.
### getDefaultAssignmentView() {#getDefaultAssignmentView--}
```
public static ProjectView getDefaultAssignmentView()
```


Incluye columnas Uid, nombre de tarea, nombre de recurso, trabajo y duración de asignación.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn).
### getDefaultGanttChartView() {#getDefaultGanttChartView--}
```
public static ProjectView getDefaultGanttChartView()
```


Incluye columnas de tarea id, indicadores, nombre, duración, inicio y fin.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
### getDefaultResourceSheetView() {#getDefaultResourceSheetView--}
```
public static ProjectView getDefaultResourceSheetView()
```


Incluye columnas de recurso Uid, nombre del recurso, tipo, etiqueta de material, iniciales, grupo, unidades máximas, tarifa estándar, tarifa de horas extra, costo por uso, acumulado en, calendario base y código de recurso.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultResourceUsageView() {#getDefaultResourceUsageView--}
```
public static ProjectView getDefaultResourceUsageView()
```


Incluye columnas de recurso de trabajo uid, nombre, inicio, fin y trabajo.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultTaskSheetView() {#getDefaultTaskSheetView--}
```
public static ProjectView getDefaultTaskSheetView()
```


Incluye columnas de tarea id, indicadores, nombre, duración, inicio, fin, predecesores y nombres de recursos.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
