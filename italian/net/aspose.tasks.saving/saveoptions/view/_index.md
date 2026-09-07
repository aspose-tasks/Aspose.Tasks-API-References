---
title: "SaveOptions.View"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà SaveOptions. Ottiene o imposta un elenco delle colonne della vista da renderizzare (GanttChartColumn). Se non impostato, vengono renderizzate solo le ID delle attività, i nomi delle attività, l'inizio e la fine. Se entrambe le proprietà View e ViewSettings sono impostate, le colonne da View sovrascrivono le colonne da ViewSettings."
type: docs
weight: 230
url: /it/net/aspose.tasks.saving/saveoptions/view/
---
## SaveOptions.View property

Ottiene o imposta un elenco delle colonne della vista da renderizzare ([`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/)). Se non impostato, vengono renderizzate solo le ID delle attività, i nomi delle attività, l'inizio e la fine. Se entrambe le proprietà View e [`ViewSettings`](../viewsettings/) sono impostate, le colonne da View sovrascrivono le colonne da ViewSettings.

```csharp
public ProjectView View { get; set; }
```

## Esempi

Mostra come aggiungere colonne della vista da esportare durante l'esportazione del progetto.

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
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


