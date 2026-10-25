---
title: "XlsxOptions"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Permite especificar opciones adicionales al renderizar páginas de proyecto a XLSX."
type: docs
weight: 368
url: /es/java/com.aspose.tasks/xlsxoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class XlsxOptions extends SimpleSaveOptions
```

Permite especificar opciones adicionales al renderizar páginas de proyecto a XLSX.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [XlsxOptions()](#XlsxOptions--) | Inicializa una nueva instancia de la clase [XlsxOptions](../../com.aspose.tasks/xlsxoptions) que puede usarse para guardar el proyecto en formato XLSX. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getAssignmentView()](#getAssignmentView--) | Obtiene una lista de las columnas de vista de asignaciones para renderizar ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [getEncoding()](#getEncoding--) | Obtiene la codificación del archivo XLSX resultante. |
| [getResourceView()](#getResourceView--) | Obtiene una lista de las columnas de vista de recursos para renderizar ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [getView()](#getView--) | Obtiene una lista de las columnas de vista ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) para guardar en formato XLSX. |
| [setAssignmentView(ProjectView value)](#setAssignmentView-com.aspose.tasks.ProjectView-) | Establece una lista de las columnas de vista de asignaciones para renderizar ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Establece la codificación del archivo XLSX resultante. |
| [setResourceView(ProjectView value)](#setResourceView-com.aspose.tasks.ProjectView-) | Establece una lista de las columnas de vista de recursos para renderizar ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Establece una lista de las columnas de vista ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) para guardar en formato XLSX. |
### XlsxOptions() {#XlsxOptions--}
```
public XlsxOptions()
```


Inicializa una nueva instancia de la clase [XlsxOptions](../../com.aspose.tasks/xlsxoptions) que puede usarse para guardar el proyecto en formato XLSX.

### getAssignmentView() {#getAssignmentView--}
```
public final ProjectView getAssignmentView()
```


Obtiene una lista de las columnas de vista de asignaciones para renderizar ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Obtiene la codificación del archivo XLSX resultante. El valor predeterminado es java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8.

**Returns:**
java.nio.charset.Charset - la codificación del archivo XLSX resultante.
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


Obtiene una lista de las columnas de vista ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) para guardar en formato XLSX. Si no se establece, se guardan las columnas predeterminadas.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setAssignmentView(ProjectView value) {#setAssignmentView-com.aspose.tasks.ProjectView-}
```
public final void setAssignmentView(ProjectView value)
```


Establece una lista de las columnas de vista de asignaciones para renderizar ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | una lista de las columnas de vista de asignaciones para renderizar ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Establece la codificación del archivo XLSX resultante. El valor predeterminado es java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.nio.charset.Charset | la codificación del archivo XLSX resultante. |

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


Establece una lista de las columnas de vista ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) para guardar en formato XLSX. Si no se establece, se guardan las columnas predeterminadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | una lista de las columnas de vista ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) para guardar en formato XLSX. |

