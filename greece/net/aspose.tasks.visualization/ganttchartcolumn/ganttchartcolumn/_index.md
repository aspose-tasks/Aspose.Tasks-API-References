---
title: "GanttChartColumn.GanttChartColumn"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής GanttChartColumn. Αρχικοποιεί μια νέα παρουσία της κλάσης GanttChartColumn"
type: docs
weight: 10
url: /el/net/aspose.tasks.visualization/ganttchartcolumn/ganttchartcolumn/
---
## GanttChartColumn(string, int, TaskToColumnTextConverter, Field) {#constructor_3}

Αρχικοποιεί μια νέα παρουσία της κλάσης GanttChartColumn.

```csharp
public GanttChartColumn(string name, int width, TaskToColumnTextConverter converter, Field field)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Όνομα στήλης. |
| πλάτος | Int32 | Πλάτος στήλης σε εικονοστοιχεία. |
| μετατροπέας | TaskToColumnTextConverter | Μετατροπέας δεδομένων εργασίας σε κείμενο στήλης. |
| πεδίο | Πεδίο | Πεδίο στήλης. |

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

* delegate [TaskToColumnTextConverter](../../tasktocolumntextconverter/)
* enum [Field](../../../aspose.tasks/field/)
* class [GanttChartColumn](../)
* namespace [Aspose.Tasks.Visualization](../../ganttchartcolumn/)
* assembly [Aspose.Tasks](../../../)

---

## GanttChartColumn(string, int, TaskToColumnTextConverter) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία της κλάσης GanttChartColumn.

```csharp
public GanttChartColumn(string name, int width, TaskToColumnTextConverter converter)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Όνομα στήλης. |
| πλάτος | Int32 | Πλάτος στήλης σε εικονοστοιχεία. |
| μετατροπέας | TaskToColumnTextConverter | Μετατροπέας δεδομένων εργασίας σε κείμενο στήλης. |

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

* delegate [TaskToColumnTextConverter](../../tasktocolumntextconverter/)
* class [GanttChartColumn](../)
* namespace [Aspose.Tasks.Visualization](../../ganttchartcolumn/)
* assembly [Aspose.Tasks](../../../)

---

## GanttChartColumn(int, Field) {#constructor}

Αρχικοποιεί μια νέα παρουσία της κλάσης GanttChartColumn.

```csharp
public GanttChartColumn(int width, Field field)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| πλάτος | Int32 | Πλάτος στήλης σε εικονοστοιχεία. |
| πεδίο | Πεδίο | Πεδίο στήλης. |

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

* enum [Field](../../../aspose.tasks/field/)
* class [GanttChartColumn](../)
* namespace [Aspose.Tasks.Visualization](../../ganttchartcolumn/)
* assembly [Aspose.Tasks](../../../)

---

## GanttChartColumn(string, int, Field) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης GanttChartColumn.

```csharp
public GanttChartColumn(string name, int width, Field field)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Όνομα στήλης. |
| πλάτος | Int32 | Πλάτος στήλης σε εικονοστοιχεία. |
| πεδίο | Πεδίο | Πεδίο στήλης. |

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

* enum [Field](../../../aspose.tasks/field/)
* class [GanttChartColumn](../)
* namespace [Aspose.Tasks.Visualization](../../ganttchartcolumn/)
* assembly [Aspose.Tasks](../../../)


