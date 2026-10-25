---
title: "Clase Spreadsheet2003SaveOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Saving.Spreadsheet2003SaveOptions. Permite especificar opciones adicionales al renderizar páginas del proyecto a Spreadsheet2003"
type: docs
weight: 2220
url: /es/net/aspose.tasks.saving/spreadsheet2003saveoptions/
---
## Spreadsheet2003SaveOptions class

Permite especificar opciones adicionales al renderizar páginas del proyecto a Spreadsheet2003.

```csharp
public class Spreadsheet2003SaveOptions : SimpleSaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Spreadsheet2003SaveOptions](spreadsheet2003saveoptions/)() | Inicializa una nueva instancia de la clase `Spreadsheet2003SaveOptions`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AssignmentView](../../aspose.tasks.saving/spreadsheet2003saveoptions/assignmentview/) { get; set; } | Obtiene o establece una lista de las columnas de vista de asignaciones a renderizar ([`AssignmentViewColumn`](../../aspose.tasks.visualization/assignmentviewcolumn/)). |
| [ResourceView](../../aspose.tasks.saving/spreadsheet2003saveoptions/resourceview/) { get; set; } | Obtiene o establece una lista de las columnas de vista de recursos a renderizar ([`ResourceViewColumn`](../../aspose.tasks.visualization/resourceviewcolumn/)). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Obtiene o establece el formato en el que se guardará el documento si se utiliza este objeto de opciones de guardado. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Obtiene o establece el comparador para ordenar tareas en el diagrama de Gantt y en el diagrama de hoja de tareas. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Obtiene o establece la condición que se utiliza para filtrar las tareas renderizadas en los diagramas de Gantt, hoja de tareas y uso de tareas. |
| [View](../../aspose.tasks.saving/spreadsheet2003saveoptions/view/) { get; set; } | Obtiene o establece una lista de las columnas de vista ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)) a guardar. Si no se establece, se guardan las columnas predeterminadas. |

## Ejemplos

Muestra cómo agregar columnas para exportar durante la exportación del proyecto al formato Spreadsheet2003.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new Spreadsheet2003SaveOptions();
var ganttChartColumn = new GanttChartColumn("WBS", 100, delegate(Task task) { return task.Get(Tsk.WBS); });
options.View.Columns.Add(ganttChartColumn);

var resourceViewColumn = new ResourceViewColumn("Cost center", 100, delegate(Resource resource) { return resource.Get(Rsc.CostCenter); });
options.ResourceView.Columns.Add(resourceViewColumn);

var assignmentViewColumn = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(assignmentViewColumn);

project.Save(OutDir + "UsingSpreadsheet2003SaveOptions_out.xml", options);
```

### Ver también

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


