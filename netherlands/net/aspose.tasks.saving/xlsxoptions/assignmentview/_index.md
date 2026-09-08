---
title: "XlsxOptions.AssignmentView"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "XlsxOptions eigenschap. Haalt een lijst op of stelt een lijst in van de kolommen voor de weergave van opdrachten om AssignmentViewColumn te renderen"
type: docs
weight: 20
url: /nl/net/aspose.tasks.saving/xlsxoptions/assignmentview/
---
## XlsxOptions.AssignmentView property

Haalt een lijst op of stelt deze in van de kolommen van de opdrachtenweergave die moeten worden gerenderd ([`AssignmentViewColumn`](../../../aspose.tasks.visualization/assignmentviewcolumn/)).

```csharp
public ProjectView AssignmentView { get; set; }
```

## Voorbeelden

Toont hoe een project op te slaan in een XLSX-bestand door gebruik te maken van &lt;see cref="P:Aspose.Tasks.Saving.XlsxOptions"&gt;Days&lt;/see&gt; opties.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new XlsxOptions();

// Voeg gewenste Gantt Chart kolommen toe
var col = new GanttChartColumn("WBS", 100, delegate(Task task) { return task.Get(Tsk.WBS); });
options.View.Columns.Add(col);

// Voeg gewenste resource view kolommen toe
var rscCol = new ResourceViewColumn("Cost center", 100, delegate(Resource resource) { return resource.Get(Rsc.CostCenter); });
options.ResourceView.Columns.Add(rscCol);

// Voeg gewenste assignment view kolommen toe
var assnCol = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(assnCol);

// stel codering in
options.Encoding = Encoding.Unicode;

project.Save(OutDir + "UsingXlsxOptions_out.xlsx", options);
```

### Zie ook

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [XlsxOptions](../)
* namespace [Aspose.Tasks.Saving](../../xlsxoptions/)
* assembly [Aspose.Tasks](../../../)


