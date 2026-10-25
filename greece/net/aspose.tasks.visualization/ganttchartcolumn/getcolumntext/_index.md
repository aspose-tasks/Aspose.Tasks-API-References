---
title: "GanttChartColumn.GetColumnText"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "GanttChartColumn μέθοδος. Μετατρέπει την τρέχουσα εργασία σε κείμενο στήλης."
type: docs
weight: 30
url: /el/net/aspose.tasks.visualization/ganttchartcolumn/getcolumntext/
---
## GanttChartColumn.GetColumnText method

Μετατρέπει την τρέχουσα εργασία σε κείμενο στήλης.

```csharp
public string GetColumnText(Task task)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| εργασία | Εργασία | Τρέχουσα εργασία. |

### Τιμή Επιστροφής

Το κείμενο στήλης.

## Παραδείγματα

Δείχνει πώς να προσθέσετε στήλες προβολής διαγράμματος Gantt για εξαγωγή.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var task = project.RootTask.Children.GetById(1);

var columns = new List<ViewColumn>
{
    new GanttChartColumn(20, Field.TaskUniqueID),
    new GanttChartColumn("Name", 150, Field.TaskName),
    new GanttChartColumn("Start", 100, Field.TaskStart),
    new GanttChartColumn("End", 100, Field.TaskFinish),
    new GanttChartColumn("R-Initials", 100, Field.TaskResourceInitials),
    new GanttChartColumn("R-Names", 100, Field.TaskResourceNames),
    new GanttChartColumn("Work", 50, Field.TaskWork),
    new GanttChartColumn(
        "Cost", 
        80,
        delegate(Task t)
        {
            return t.Get(Tsk.Cost).ToString(CultureInfo.InvariantCulture);
        }),
    new GanttChartColumn(
        "Actual Cost", 
        80,
        delegate(Task t)
        {
            return t.Get(Tsk.ActualCost).ToString(CultureInfo.InvariantCulture);
        },
        Field.TaskActualCost)
};

// επανάληψη στις στήλες
foreach (var column in columns)
{
    var col = (GanttChartColumn)column;
    Console.WriteLine("Column Name: " + col.Name);
    Console.WriteLine("Column Field: " + col.Field);
    Console.WriteLine("Column Text: " + col.GetColumnText(task));
    Console.WriteLine();
}

var options = new CsvOptions
{
    View = new ProjectView(columns)
};

project.Save(OutDir + "WorkWithGanttChartColumn_out.csv", options);
```

### Δείτε επίσης

* class [Task](../../../aspose.tasks/task/)
* class [GanttChartColumn](../)
* namespace [Aspose.Tasks.Visualization](../../ganttchartcolumn/)
* assembly [Aspose.Tasks](../../../)


