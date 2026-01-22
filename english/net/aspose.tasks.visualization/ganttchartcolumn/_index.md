---
title: Class GanttChartColumn
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.GanttChartColumn class. Projects view class
type: docs
weight: 3060
url: /net/aspose.tasks.visualization/ganttchartcolumn/
---
## GanttChartColumn class

Project's view class

```csharp
public sealed class GanttChartColumn : ViewColumn
```

## Constructors

| Name | Description |
| --- | --- |
| [GanttChartColumn](ganttchartcolumn/#constructor)(int, Field) | Initializes a new instance of the GanttChartColumn class. |
| [GanttChartColumn](ganttchartcolumn/#constructor_1)(string, int, Field) | Initializes a new instance of the GanttChartColumn class. |
| [GanttChartColumn](ganttchartcolumn/#constructor_2)(string, int, TaskToColumnTextConverter) | Initializes a new instance of the GanttChartColumn class. |
| [GanttChartColumn](ganttchartcolumn/#constructor_3)(string, int, TaskToColumnTextConverter, Field) | Initializes a new instance of the GanttChartColumn class. |

## Properties

| Name | Description |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/ganttchartcolumn/field/) { get; set; } | Column field. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Gets the column name. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Gets or sets alignment of the text (can be one of the values of the [`HorizontalStringAlignment`](../horizontalstringalignment/) enumeration). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Gets or sets the callback which can be used to customize the appearance of the column's cells. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Gets the column width. |

## Methods

| Name | Description |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/ganttchartcolumn/getcolumntext/)(Task) | Converts current task to the column text. |

## Examples

Shows how to add Gantt chart view columns to be exported.

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

// iterate over columns
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

### See Also

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


