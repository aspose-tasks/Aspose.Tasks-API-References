---
title: "ProjectView.ProjectView"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ProjectView-constructor. Initialiseert een nieuw exemplaar van de ProjectView-klasse"
type: docs
weight: 10
url: /nl/net/aspose.tasks.visualization/projectview/projectview/
---
## ProjectView constructor

Initialiseert een nieuw exemplaar van de [`ProjectView`](../) klasse.

```csharp
public ProjectView(IEnumerable<ViewColumn> columns)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| kolommen | IEnumerable`1 | Een lijst van de weergavekolommen. |

## Voorbeelden

Toont hoe een project op te slaan met een weergave met een aangepaste set kolommen.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var options = new PdfSaveOptions();
var columns = new List<ViewColumn>
{
    new GanttChartColumn("Name", 100, Field.TaskName),
    new GanttChartColumn("Start", 100, Field.TaskStart),
    new GanttChartColumn("Finish", 100, Field.TaskFinish),
    new GanttChartColumn("Cost2", 80, Field.TaskCost2),
    new GanttChartColumn("Number6", 80, Field.TaskNumber6),
    new GanttChartColumn("Date6", 80, Field.TaskDate6),
    new GanttChartColumn("Flag6", 80, Field.TaskFlag6),
    new GanttChartColumn("Flag18", 80, Field.TaskFlag18),
    new GanttChartColumn("Duration6", 80, Field.TaskDuration6)
};
options.View = new ProjectView(columns);

// itereren over weergavekolommen
foreach (var column in options.View.Columns)
{
    Console.WriteLine("Column Name: " + column.Name);
}

options.PresentationFormat = PresentationFormat.TaskUsage;
project.Save(OutDir + "TaskUsageProjectView_Columns.pdf", options);
```

### Zie ook

* class [ViewColumn](../../viewcolumn/)
* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


