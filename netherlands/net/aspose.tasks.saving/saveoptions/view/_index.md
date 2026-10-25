---
title: "SaveOptions.View"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "SaveOptions-eigenschap. Haalt een lijst op of stelt deze in van de view-kolommen die moeten worden gerenderd (GanttChartColumn). Indien niet ingesteld, worden alleen taak‑ID's, taaknamen, start‑ en eindtijd gerenderd. Als zowel View- als ViewSettings‑eigenschappen zijn ingesteld, hebben kolommen van View voorrang boven kolommen van ViewSettings."
type: docs
weight: 230
url: /nl/net/aspose.tasks.saving/saveoptions/view/
---
## SaveOptions.View property

Haalt een lijst op of stelt deze in van de view‑kolommen die moeten worden gerenderd ([`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/)). Indien niet ingesteld, worden alleen taak‑ID's, taaknamen, start‑ en eindtijd gerenderd. Als zowel View als de [`ViewSettings`](../viewsettings/) eigenschappen zijn ingesteld, hebben kolommen van View voorrang boven kolommen van ViewSettings.

```csharp
public ProjectView View { get; set; }
```

## Voorbeelden

Toont hoe kolommen van de view toe te voegen die tijdens het exporteren van een project geëxporteerd moeten worden.

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
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


