---
title: "ProjectView.Columns"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ProjectView. Λαμβάνει τις στήλες προβολής του έργου"
type: docs
weight: 70
url: /el/net/aspose.tasks.visualization/projectview/columns/
---
## ProjectView.Columns property

Λαμβάνει τις στήλες προβολής έργου.

```csharp
public List<ViewColumn> Columns { get; }
```

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε ένα έργο με προβολή με προσαρμοσμένο σύνολο στηλών.

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

// Επανάληψη στις στήλες προβολής
foreach (var column in options.View.Columns)
{
    Console.WriteLine("Column Name: " + column.Name);
}

options.PresentationFormat = PresentationFormat.TaskUsage;
project.Save(OutDir + "TaskUsageProjectView_Columns.pdf", options);
```

### Δείτε επίσης

* class [ViewColumn](../../viewcolumn/)
* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


