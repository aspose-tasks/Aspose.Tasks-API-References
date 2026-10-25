---
title: "Spreadsheet2003SaveOptions.Spreadsheet2003SaveOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Spreadsheet2003SaveOptions constructor. Initialiseert een nieuw exemplaar van de Spreadsheet2003SaveOptions-klasse"
type: docs
weight: 10
url: /nl/net/aspose.tasks.saving/spreadsheet2003saveoptions/spreadsheet2003saveoptions/
---
## Spreadsheet2003SaveOptions constructor

Initialiseert een nieuw exemplaar van de [`Spreadsheet2003SaveOptions`](../) klasse.

```csharp
public Spreadsheet2003SaveOptions()
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

* class [Spreadsheet2003SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../spreadsheet2003saveoptions/)
* assembly [Aspose.Tasks](../../../)


