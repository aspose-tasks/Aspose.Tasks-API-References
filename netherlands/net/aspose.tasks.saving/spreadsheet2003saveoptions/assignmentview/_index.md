---
title: "Spreadsheet2003SaveOptions.AssignmentView"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Spreadsheet2003SaveOptions eigenschap. Haalt een lijst op of stelt deze in van de kolommen van de opdrachtenweergave die moeten worden gerenderd AssignmentViewColumn."
type: docs
weight: 20
url: /nl/net/aspose.tasks.saving/spreadsheet2003saveoptions/assignmentview/
---
## Spreadsheet2003SaveOptions.AssignmentView property

Haalt een lijst op of stelt deze in van de kolommen van de opdrachtenweergave die moeten worden gerenderd ([`AssignmentViewColumn`](../../../aspose.tasks.visualization/assignmentviewcolumn/)).

```csharp
public ProjectView AssignmentView { get; set; }
```

## Voorbeelden

Toont hoe kolommen toe te voegen die geëxporteerd moeten worden tijdens het exporteren van een project naar Spreadsheet2003-indeling.

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

### Zie ook

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [Spreadsheet2003SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../spreadsheet2003saveoptions/)
* assembly [Aspose.Tasks](../../../)


