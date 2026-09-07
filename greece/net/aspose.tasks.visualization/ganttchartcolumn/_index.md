---
title: "Κλάση GanttChartColumn"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.Visualization.GanttChartColumn. Κλάση προβολής Projects"
type: docs
weight: 3090
url: /el/net/aspose.tasks.visualization/ganttchartcolumn/
---
## GanttChartColumn class

Κλάση προβολής του έργου

```csharp
public sealed class GanttChartColumn : ViewColumn
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [GanttChartColumn](ganttchartcolumn/#constructor)(int, Field) | Αρχικοποιεί μια νέα παρουσία της κλάσης GanttChartColumn. |
| [GanttChartColumn](ganttchartcolumn/#constructor_1)(string, int, Field) | Αρχικοποιεί μια νέα παρουσία της κλάσης GanttChartColumn. |
| [GanttChartColumn](ganttchartcolumn/#constructor_2)(string, int, TaskToColumnTextConverter) | Αρχικοποιεί μια νέα παρουσία της κλάσης GanttChartColumn. |
| [GanttChartColumn](ganttchartcolumn/#constructor_3)(string, int, TaskToColumnTextConverter, Field) | Αρχικοποιεί μια νέα παρουσία της κλάσης GanttChartColumn. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/ganttchartcolumn/field/) { get; set; } | Πεδίο στήλης. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Λαμβάνει το όνομα της στήλης. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Λαμβάνει ή ορίζει την ευθυγράμμιση του κειμένου (μπορεί να είναι μία από τις τιμές της απαρίθμησης [`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Λαμβάνει ή ορίζει την κλήση επιστροφής (callback) που μπορεί να χρησιμοποιηθεί για την προσαρμογή της εμφάνισης των κελιών της στήλης. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Λαμβάνει το πλάτος της στήλης. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/ganttchartcolumn/getcolumntext/)(Task) | Μετατρέπει την τρέχουσα εργασία σε κείμενο στήλης. |

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

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


