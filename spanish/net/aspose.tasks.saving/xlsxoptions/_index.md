---
title: "Clase XlsxOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Saving.XlsxOptions. Permite especificar opciones adicionales al renderizar páginas de proyecto a XLSX"
type: docs
weight: 2270
url: /es/net/aspose.tasks.saving/xlsxoptions/
---
## XlsxOptions class

Permite especificar opciones adicionales al renderizar páginas de proyecto a XLSX.

```csharp
public class XlsxOptions : SimpleSaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [XlsxOptions](xlsxoptions/)() | Inicializa una nueva instancia de la clase `XlsxOptions` que puede usarse para guardar el proyecto en formato XLSX. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AssignmentView](../../aspose.tasks.saving/xlsxoptions/assignmentview/) { get; set; } | Obtiene o establece una lista de las columnas de vista de asignaciones a renderizar ([`AssignmentViewColumn`](../../aspose.tasks.visualization/assignmentviewcolumn/)). |
| [Encoding](../../aspose.tasks.saving/xlsxoptions/encoding/) { get; set; } | Obtiene o establece la codificación del archivo XLSX resultante. El valor predeterminado es UTF8. |
| [ResourceView](../../aspose.tasks.saving/xlsxoptions/resourceview/) { get; set; } | Obtiene o establece una lista de las columnas de vista de recursos a renderizar ([`ResourceViewColumn`](../../aspose.tasks.visualization/resourceviewcolumn/)). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Obtiene o establece el formato en el que se guardará el documento si se utiliza este objeto de opciones de guardado. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Obtiene o establece el comparador para ordenar tareas en el diagrama de Gantt y en el diagrama de hoja de tareas. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Obtiene o establece la condición que se utiliza para filtrar las tareas renderizadas en los diagramas de Gantt, hoja de tareas y uso de tareas. |
| [View](../../aspose.tasks.saving/xlsxoptions/view/) { get; set; } | Obtiene o establece una lista de las columnas de vista ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)) para guardar en formato XLSX. Si no se establece, se guardan las columnas predeterminadas. |

## Ejemplos

Muestra cómo guardar un proyecto en un archivo XLSX usando las opciones &lt;see cref=\"P:Aspose.Tasks.Saving.XlsxOptions\"&gt;Days&lt;/see&gt;.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new XlsxOptions();

// Agregar columnas deseadas del diagrama Gantt
var col = new GanttChartColumn("WBS", 100, delegate(Task task) { return task.Get(Tsk.WBS); });
options.View.Columns.Add(col);

// Agregar columnas deseadas de la vista de recursos
var rscCol = new ResourceViewColumn("Cost center", 100, delegate(Resource resource) { return resource.Get(Rsc.CostCenter); });
options.ResourceView.Columns.Add(rscCol);

// Agregar columnas deseadas de la vista de asignaciones
var assnCol = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(assnCol);

// establecer codificación
options.Encoding = Encoding.Unicode;

project.Save(OutDir + "UsingXlsxOptions_out.xlsx", options);
```

### Ver también

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


