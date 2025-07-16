---
title: Class GanttBarStyle
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.GanttBarStyle class. Represents a bar style used by MSP in Gantt Chart view
type: docs
weight: 2990
url: /net/aspose.tasks.visualization/ganttbarstyle/
---
## GanttBarStyle class

Represents a bar style used by MSP in Gantt Chart view.

```csharp
public class GanttBarStyle
```

## Constructors

| Name | Description |
| --- | --- |
| [GanttBarStyle](ganttbarstyle/)() | Initializes a new instance of the `GanttBarStyle` class. |

## Properties

| Name | Description |
| --- | --- |
| [BottomBarTextConverter](../../aspose.tasks.visualization/ganttbarstyle/bottombartextconverter/) { get; set; } | Gets or sets user-defined converter to get text to render on the bottom of the task's bar. Overrides the value of [`BottomField`](./bottomfield/) property. |
| [BottomField](../../aspose.tasks.visualization/ganttbarstyle/bottomfield/) { get; set; } | Gets or sets data to be displayed on the bottom of the bar. [`Field`](../../aspose.tasks/field/). |
| [EndShape](../../aspose.tasks.visualization/ganttbarstyle/endshape/) { get; set; } | Gets or sets an end shape of the bar. |
| [EndShapeColor](../../aspose.tasks.visualization/ganttbarstyle/endshapecolor/) { get; set; } | Gets or sets a color of the end shape. |
| [EndShapeType](../../aspose.tasks.visualization/ganttbarstyle/endshapetype/) { get; set; } | Gets or sets a type of the end shape. [`GanttBarType`](../ganttbartype/). |
| [From](../../aspose.tasks.visualization/ganttbarstyle/from/) { get; set; } | Gets or sets a start point position of the gantt bar. [`Field`](../../aspose.tasks/field/). |
| [InsideBarTextConverter](../../aspose.tasks.visualization/ganttbarstyle/insidebartextconverter/) { get; set; } | Gets or sets user-defined converter to get text to render inside of the task's bar. Overrides the value of [`InsideField`](./insidefield/) property. |
| [InsideField](../../aspose.tasks.visualization/ganttbarstyle/insidefield/) { get; set; } | Gets or sets data to be displayed inside of the bar. [`Field`](../../aspose.tasks/field/). |
| [LeftBarTextConverter](../../aspose.tasks.visualization/ganttbarstyle/leftbartextconverter/) { get; set; } | Gets or sets user-defined converter to get text to render on the left of the task's bar. Overrides the value of [`LeftField`](./leftfield/) property. Is not persisted to MPP format. |
| [LeftField](../../aspose.tasks.visualization/ganttbarstyle/leftfield/) { get; set; } | Gets or sets data to be displayed on the left of the bar. [`Field`](../../aspose.tasks/field/). |
| [MiddleFillPattern](../../aspose.tasks.visualization/ganttbarstyle/middlefillpattern/) { get; set; } | Gets or sets a fill pattern of the gantt bar. |
| [MiddleShape](../../aspose.tasks.visualization/ganttbarstyle/middleshape/) { get; set; } | Gets or sets a middle shape of the bar. |
| [MiddleShapeColor](../../aspose.tasks.visualization/ganttbarstyle/middleshapecolor/) { get; set; } | Gets or sets a color of the middle shape. |
| [Name](../../aspose.tasks.visualization/ganttbarstyle/name/) { get; set; } | Gets or sets a name of the style. |
| [ParentStyle](../../aspose.tasks.visualization/ganttbarstyle/parentstyle/) { get; set; } | Gets or sets parent (or common) style for custom task-specific style. |
| [RightBarTextConverter](../../aspose.tasks.visualization/ganttbarstyle/rightbartextconverter/) { get; set; } | Gets or sets user-defined converter to get text to render on the right of the task's bar. Overrides the value of [`RightField`](./rightfield/) property. |
| [RightField](../../aspose.tasks.visualization/ganttbarstyle/rightfield/) { get; set; } | Gets or sets data to be displayed on the right of the bar. [`Field`](../../aspose.tasks/field/). |
| [Row](../../aspose.tasks.visualization/ganttbarstyle/row/) { get; set; } | Gets or sets a row number.  Can be from 1 to 4 (1 is default value). |
| [ShowForCategories](../../aspose.tasks.visualization/ganttbarstyle/showforcategories/) { get; set; } | Gets or sets task categories for which the style is applied. Is applicable for parent (or common) styles of bars in Gantt chart (see [`BarStyles`](../../aspose.tasks/ganttchartview/barstyles/)). |
| [ShowForTaskUid](../../aspose.tasks.visualization/ganttbarstyle/showfortaskuid/) { get; set; } | Gets or sets Unique Id of a task for which the style is applied. Is applicable for task-specific styles of bars in Gantt chart (see [`CustomBarStyles`](../../aspose.tasks/ganttchartview/custombarstyles/)). |
| [StartShape](../../aspose.tasks.visualization/ganttbarstyle/startshape/) { get; set; } | Gets or sets a start shape of the bar. |
| [StartShapeColor](../../aspose.tasks.visualization/ganttbarstyle/startshapecolor/) { get; set; } | Gets or sets a color of the start shape. |
| [StartShapeType](../../aspose.tasks.visualization/ganttbarstyle/startshapetype/) { get; set; } | Gets or sets a type of the start shape. |
| [To](../../aspose.tasks.visualization/ganttbarstyle/to/) { get; set; } | Gets or sets a finish point position of the gantt bar. |
| [TopBarTextConverter](../../aspose.tasks.visualization/ganttbarstyle/topbartextconverter/) { get; set; } | Gets or sets user-defined converter to get text to render on the top of the task's bar. Overrides the value of [`TopField`](./topfield/) property. |
| [TopField](../../aspose.tasks.visualization/ganttbarstyle/topfield/) { get; set; } | Gets or sets data to be displayed on the top of the bar. |

## Examples

Shows how to use custom bar styles of Gantt Chart view.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var ganttChartView = (GanttChartView)project.Views.First(v => v.Name == "Gantt &Chart");
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.ViewSettings = ganttChartView;

// Bar styles can be either task-specific (located in GanttChartView.CustomBarStyles)
// of category-specific (located in GanttChartView.BarStyles)
foreach (GanttBarStyle ganttBarStyle in ganttChartView.CustomBarStyles)
{
    if (ganttBarStyle.ShowForTaskUid != 4)
    {
        continue;
    }

    // For demonstration purposes we are modifying style for Task with Unique ID = 4
    // Here we set field (TaskName) to render to the left of the task bar.
    ganttBarStyle.LeftField = Field.TaskName;
    // Here we set custom converter to control which text should be rendered inside the task bar.
    ganttBarStyle.InsideBarTextConverter = task => "Hours rem.: " + (int)task.Get(Tsk.RemainingWork).TimeSpan.TotalHours;

    ganttBarStyle.MiddleShapeColor = Color.Green;
    ganttBarStyle.MiddleShape = GanttBarMiddleShape.LineTop;
    ganttBarStyle.StartShape = GanttBarEndShape.LeftBracket;
    ganttBarStyle.StartShapeColor = Color.Aqua;
    ganttBarStyle.EndShape = GanttBarEndShape.RightBracket;
    ganttBarStyle.EndShapeColor = Color.Aquamarine;
}

foreach (GanttBarStyle ganttBarStyle in ganttChartView.BarStyles)
{
    if (!ganttBarStyle.ShowForCategories.Contains(GanttBarShowFor.Milestone))
    {
        continue;
    }

    // For demonstration purposes we are modifying styles applicable to milestone tasks.

    ganttBarStyle.StartShape = GanttBarEndShape.Diamond;
    ganttBarStyle.RightField = Field.TaskActualFinish;
    ganttBarStyle.TopBarTextConverter = task => task.Get(Tsk.ActualStart).Day.ToString();
}

project.Save(OutDir + "WorkWithGanttChartViewBarStyles_out.pdf", saveOptions);
```

Shows how to read custom bar styles of a view.

```csharp
var project = new Project(DataDir + "CustomBarStyle.mpp");

var view = (GanttChartView)project.DefaultView;
Console.WriteLine("Custom bar styles count: {0}", view.CustomBarStyles.Count);

var style1 = view.CustomBarStyles[0];
Console.WriteLine("Style1.ParentStyle Name: {0}", style1.ParentStyle.Name);
Console.WriteLine("Style1.LeftField: {0}", style1.LeftField);
Console.WriteLine("Style1.RightField: {0}", style1.RightField);
Console.WriteLine("Style1.TopField: {0}", style1.TopField);
Console.WriteLine("Style1.BottomField: {0}", style1.BottomField);
Console.WriteLine("Style1.InsideField: {0}", style1.InsideField);
Console.WriteLine("Style1.From: {0}", style1.From);
Console.WriteLine("Style1.To: {0}", style1.To);
Console.WriteLine("Style1.Row: {0}", style1.Row);

var style2 = view.CustomBarStyles[1];
Console.WriteLine("Style2.LeftField: {0}", style2.LeftField);
Console.WriteLine("Style2.RightField: {0}", style2.RightField);
Console.WriteLine("Style2.TopField: {0}", style2.TopField);
Console.WriteLine("Style2.BottomField: {0}", style2.BottomField);
Console.WriteLine("Style2.InsideField: {0}", style2.InsideField);
Console.WriteLine("Style2.From: {0}", style2.From);
Console.WriteLine("Style2.To: {0}", style2.To);
Console.WriteLine("Style2.Row: {0}", style1.Row);

var style3 = view.CustomBarStyles[2];
Console.WriteLine("Style3.LeftField: {0}", style3.LeftField);
Console.WriteLine("Style3.RightField: {0}", style3.RightField);
Console.WriteLine("Style3.TopField: {0}", style3.TopField);
Console.WriteLine("Style3.BottomField: {0}", style3.BottomField);
Console.WriteLine("Style3.InsideField: {0}", style3.InsideField);

Console.WriteLine("Style3.StartShape: {0}", style3.StartShape);
Console.WriteLine("Style3.StartShapeType: {0}", style3.StartShapeType);
Console.WriteLine("Style3.StartShapeColor: {0}", style3.StartShapeColor);

Console.WriteLine("Style3.EndShape: {0}", style3.EndShape);
Console.WriteLine("Style3.EndShapeType: {0}", style3.EndShapeType);
Console.WriteLine("Style3.EndShapeColor: {0}", style3.EndShapeColor);

Console.WriteLine("Style3.MiddleShape: {0}", style3.MiddleShape);
Console.WriteLine("Style3.MiddleFillPattern: {0}", style3.MiddleFillPattern);
Console.WriteLine("Style3.MiddleShapeColor: {0}", style3.MiddleShapeColor);
Console.WriteLine("Style3.From: {0}", style3.From);
Console.WriteLine("Style3.To: {0}", style3.To);
Console.WriteLine("Style3.Row: {0}", style1.Row);
```

### See Also

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


