---
title: "Spreadsheet2003SaveOptions.AssignmentView"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Spreadsheet2003SaveOptions property. Ottiene o imposta un elenco delle colonne della vista delle assegnazioni da renderizzare AssignmentViewColumn"
type: docs
weight: 20
url: /it/net/aspose.tasks.saving/spreadsheet2003saveoptions/assignmentview/
---
## Spreadsheet2003SaveOptions.AssignmentView property

Ottiene o imposta un elenco delle colonne della vista delle assegnazioni da renderizzare ([`AssignmentViewColumn`](../../../aspose.tasks.visualization/assignmentviewcolumn/)).

```csharp
public ProjectView AssignmentView { get; set; }
```

## Esempi

Mostra come aggiungere colonne da esportare durante l'esportazione del progetto nel formato Spreadsheet2003.

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

### Vedi anche

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [Spreadsheet2003SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../spreadsheet2003saveoptions/)
* assembly [Aspose.Tasks](../../../)


