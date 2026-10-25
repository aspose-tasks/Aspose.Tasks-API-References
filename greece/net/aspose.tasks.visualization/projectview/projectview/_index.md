---
title: "ProjectView.ProjectView"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής ProjectView. Αρχικοποιεί ένα νέο αντικείμενο της κλάσης ProjectView"
type: docs
weight: 10
url: /el/net/aspose.tasks.visualization/projectview/projectview/
---
## ProjectView constructor

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`ProjectView`](../).

```csharp
public ProjectView(IEnumerable<ViewColumn> columns)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| στήλες | IEnumerable`1 | Μια λίστα των στηλών προβολής. |

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


