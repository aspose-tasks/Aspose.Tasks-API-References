---
title: "Klasse GanttChartColumn"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.GanttChartColumn-klasse. Projecten weergaveklasse"
type: docs
weight: 3090
url: /nl/net/aspose.tasks.visualization/ganttchartcolumn/
---
## GanttChartColumn class

Klasse van projectweergave

```csharp
public sealed class GanttChartColumn : ViewColumn
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [GanttChartColumn](ganttchartcolumn/#constructor)(int, Field) | Initialiseert een nieuwe instantie van de GanttChartColumn-klasse. |
| [GanttChartColumn](ganttchartcolumn/#constructor_1)(string, int, Field) | Initialiseert een nieuwe instantie van de GanttChartColumn-klasse. |
| [GanttChartColumn](ganttchartcolumn/#constructor_2)(string, int, TaskToColumnTextConverter) | Initialiseert een nieuwe instantie van de GanttChartColumn-klasse. |
| [GanttChartColumn](ganttchartcolumn/#constructor_3)(string, int, TaskToColumnTextConverter, Field) | Initialiseert een nieuwe instantie van de GanttChartColumn-klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/ganttchartcolumn/field/) { get; set; } | Kolomveld. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Haalt de kolomnaam op. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Haalt de uitlijning van de tekst op of stelt deze in (kan een van de waarden van de enumeratie [`HorizontalStringAlignment`](../horizontalstringalignment/) zijn). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Haalt de callback op of stelt deze in die kan worden gebruikt om het uiterlijk van de cellen van de kolom aan te passen. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Haalt de kolombreedte op. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/ganttchartcolumn/getcolumntext/)(Task) | Converteert de huidige taak naar de kolomtekst. |

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

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


