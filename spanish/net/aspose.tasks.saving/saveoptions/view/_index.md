---
title: "SaveOptions.View"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad SaveOptions. Obtiene o establece una lista de las columnas de vista a renderizar GanttChartColumn. Si no se establece, solo se renderizan los IDs de tareas, nombres de tareas, inicio y fin. Si ambas propiedades View y ViewSettings están establecidas, las columnas de View sobrescriben a las de ViewSettings."
type: docs
weight: 230
url: /es/net/aspose.tasks.saving/saveoptions/view/
---
## SaveOptions.View property

Obtiene o establece una lista de las columnas de vista a renderizar ([`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/)). Si no se establece, solo se renderizan los IDs de tareas, nombres de tareas, inicio y fin. Si ambas propiedades View y [`ViewSettings`](../viewsettings/) están establecidas, las columnas de View sobrescriben a las de ViewSettings.

```csharp
public ProjectView View { get; set; }
```

## Ejemplos

Muestra cómo agregar columnas de vista para exportar durante la exportación del proyecto.

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

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


