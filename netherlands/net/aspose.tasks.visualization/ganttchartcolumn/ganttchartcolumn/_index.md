---
title: "GanttChartColumn.GanttChartColumn"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "GanttChartColumn constructor. Initialiseert een nieuw exemplaar van de GanttChartColumn-klasse"
type: docs
weight: 10
url: /nl/net/aspose.tasks.visualization/ganttchartcolumn/ganttchartcolumn/
---
## GanttChartColumn(string, int, TaskToColumnTextConverter, Field) {#constructor_3}

Initialiseert een nieuwe instantie van de GanttChartColumn-klasse.

```csharp
public GanttChartColumn(string name, int width, TaskToColumnTextConverter converter, Field field)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | Naam van kolom. |
| breedte | Int32 | Breedte van kolom in pixels. |
| converter | TaskToColumnTextConverter | Taakgegevens naar kolomtekstconverter. |
| veld | Veld | Kolomveld. |

## Voorbeelden

Toont hoe Gantt-diagramweergavekolommen toe te voegen die geëxporteerd moeten worden.

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

// itereren over kolommen
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

### Zie ook

* delegate [TaskToColumnTextConverter](../../tasktocolumntextconverter/)
* enum [Field](../../../aspose.tasks/field/)
* class [GanttChartColumn](../)
* namespace [Aspose.Tasks.Visualization](../../ganttchartcolumn/)
* assembly [Aspose.Tasks](../../../)

---

## GanttChartColumn(string, int, TaskToColumnTextConverter) {#constructor_2}

Initialiseert een nieuwe instantie van de GanttChartColumn-klasse.

```csharp
public GanttChartColumn(string name, int width, TaskToColumnTextConverter converter)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | Naam van kolom. |
| breedte | Int32 | Breedte van kolom in pixels. |
| converter | TaskToColumnTextConverter | Taakgegevens naar kolomtekstconverter. |

## Voorbeelden

Toont hoe Gantt-diagramweergavekolommen toe te voegen die geëxporteerd moeten worden.

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

// itereren over kolommen
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

### Zie ook

* delegate [TaskToColumnTextConverter](../../tasktocolumntextconverter/)
* class [GanttChartColumn](../)
* namespace [Aspose.Tasks.Visualization](../../ganttchartcolumn/)
* assembly [Aspose.Tasks](../../../)

---

## GanttChartColumn(int, Field) {#constructor}

Initialiseert een nieuwe instantie van de GanttChartColumn-klasse.

```csharp
public GanttChartColumn(int width, Field field)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| breedte | Int32 | Kolombreedte in pixels. |
| veld | Veld | Kolomveld. |

## Voorbeelden

Toont hoe Gantt-diagramweergavekolommen toe te voegen die geëxporteerd moeten worden.

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

// itereren over kolommen
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

### Zie ook

* enum [Field](../../../aspose.tasks/field/)
* class [GanttChartColumn](../)
* namespace [Aspose.Tasks.Visualization](../../ganttchartcolumn/)
* assembly [Aspose.Tasks](../../../)

---

## GanttChartColumn(string, int, Field) {#constructor_1}

Initialiseert een nieuwe instantie van de GanttChartColumn-klasse.

```csharp
public GanttChartColumn(string name, int width, Field field)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | Kolomnaam. |
| breedte | Int32 | Kolombreedte in pixels. |
| veld | Veld | Kolomveld. |

## Voorbeelden

Toont hoe Gantt-diagramweergavekolommen toe te voegen die geëxporteerd moeten worden.

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

// itereren over kolommen
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

### Zie ook

* enum [Field](../../../aspose.tasks/field/)
* class [GanttChartColumn](../)
* namespace [Aspose.Tasks.Visualization](../../ganttchartcolumn/)
* assembly [Aspose.Tasks](../../../)


