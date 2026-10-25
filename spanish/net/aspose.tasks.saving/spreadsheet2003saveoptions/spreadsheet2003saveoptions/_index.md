---
title: "Spreadsheet2003SaveOptions.Spreadsheet2003SaveOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor de Spreadsheet2003SaveOptions. Inicializa una nueva instancia de la clase Spreadsheet2003SaveOptions"
type: docs
weight: 10
url: /es/net/aspose.tasks.saving/spreadsheet2003saveoptions/spreadsheet2003saveoptions/
---
## Spreadsheet2003SaveOptions constructor

Inicializa una nueva instancia de la clase [`Spreadsheet2003SaveOptions`](../).

```csharp
public Spreadsheet2003SaveOptions()
```

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

* class [Spreadsheet2003SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../spreadsheet2003saveoptions/)
* assembly [Aspose.Tasks](../../../)


