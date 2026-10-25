---
title: "Spreadsheet2003SaveOptions"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Permite especificar opciones adicionales al renderizar páginas de proyecto a Spreadsheet2003."
type: docs
weight: 280
url: /es/java/com.aspose.tasks/spreadsheet2003saveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class Spreadsheet2003SaveOptions extends SimpleSaveOptions
```

Permite especificar opciones adicionales al renderizar páginas de proyecto a Spreadsheet2003.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [Spreadsheet2003SaveOptions()](#Spreadsheet2003SaveOptions--) | Inicializa una nueva instancia de la clase [Spreadsheet2003SaveOptions](../../com.aspose.tasks/spreadsheet2003saveoptions). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getAssignmentView()](#getAssignmentView--) | Obtiene una lista de las columnas de vista de asignaciones para renderizar ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [getResourceView()](#getResourceView--) | Obtiene una lista de las columnas de vista de recursos para renderizar ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [getView()](#getView--) | Obtiene una lista de las columnas de vista ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) para guardar. |
| [setAssignmentView(ProjectView value)](#setAssignmentView-com.aspose.tasks.ProjectView-) | Establece una lista de las columnas de vista de asignaciones para renderizar ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [setResourceView(ProjectView value)](#setResourceView-com.aspose.tasks.ProjectView-) | Establece una lista de las columnas de vista de recursos para renderizar ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Establece una lista de las columnas de vista ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) para guardar. |
### Spreadsheet2003SaveOptions() {#Spreadsheet2003SaveOptions--}
```
public Spreadsheet2003SaveOptions()
```


Inicializa una nueva instancia de la clase [Spreadsheet2003SaveOptions](../../com.aspose.tasks/spreadsheet2003saveoptions).

### getAssignmentView() {#getAssignmentView--}
```
public final ProjectView getAssignmentView()
```


Obtiene una lista de las columnas de vista de asignaciones para renderizar ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).
### getResourceView() {#getResourceView--}
```
public final ProjectView getResourceView()
```


Obtiene una lista de las columnas de vista de recursos para renderizar ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the resource view columns to render ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).
### getView() {#getView--}
```
public final ProjectView getView()
```


Obtiene una lista de las columnas de vista ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) para guardar. Si no se establece, se guardan las columnas predeterminadas.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save.
### setAssignmentView(ProjectView value) {#setAssignmentView-com.aspose.tasks.ProjectView-}
```
public final void setAssignmentView(ProjectView value)
```


Establece una lista de las columnas de vista de asignaciones para renderizar ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | una lista de las columnas de vista de asignaciones para renderizar ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |

### setResourceView(ProjectView value) {#setResourceView-com.aspose.tasks.ProjectView-}
```
public final void setResourceView(ProjectView value)
```


Establece una lista de las columnas de vista de recursos para renderizar ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | una lista de las columnas de vista de recursos para renderizar ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


Establece una lista de las columnas de vista ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) para guardar. Si no se establece, se guardan las columnas predeterminadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | una lista de las columnas de vista ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) para guardar. |

