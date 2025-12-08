---
title: Enum GanttBarMiddleShape
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.GanttBarMiddleShape enum. Specifies the middle shape of a bar
type: docs
weight: 3000
url: /net/aspose.tasks.visualization/ganttbarmiddleshape/
---
## GanttBarMiddleShape enumeration

Specifies the middle shape of a bar.

```csharp
public enum GanttBarMiddleShape
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| LineBottom | `7` | Indicates bottom-aligned line shape. |
| LineMiddle | `6` | Indicates center-aligned line shape. |
| LineTop | `5` | Indicates top-aligned line shape. |
| None | `0` | Indicates empty shape. |
| RectangleBar | `1` | Indicates full height rectangle bar shape. |
| RectangleBottom | `4` | Indicates Indicates bottom-aligned half height rectangle bar shape. |
| RectangleMiddle | `3` | Indicates center-aligned 1/3 height rectangle bar shape. |
| RectangleTop | `2` | Indicates top-aligned half height rectangle bar shape. |

## Examples

Shows how to set custom bar styles of Gantt Chart project view.

```csharp
public void ImplementCustomBarStyle()
{
    try
    {
        var project = new Project(DataDir + "Blank2010.mpp");
        project.RootTask.Children.Add("Task");

        var view = (GanttChartView)project.DefaultView;
        var custom = GetCustomBarStyle();

        // Add the custom bar style to the custom bar collection of the project view
        view.CustomBarStyles.Add(custom);

        SimpleSaveOptions options = new MPPSaveOptions
        {
            WriteViewData = true
        };

        project.Save(OutDir + "ImplementCustomBarStyleWriting_out.mpp", options);
    }
    catch (NotSupportedException ex)
    {
        Console.WriteLine(
            ex.Message
            + "\nThis example will only work if you apply a valid Aspose License. You can purchase full license or get 30 day temporary license from http://www.aspose.com/purchase/default.aspx.");
    }
}

public static GanttBarStyle GetCustomBarStyle()
{
    var style = new GanttBarStyle
    {
        ShowForTaskUid = 1,
        MiddleShape = GanttBarMiddleShape.RectangleBottom,
        MiddleFillPattern = GanttBarFillPattern.MediumFill,
        MiddleShapeColor = Color.Blue,

        StartShape = GanttBarEndShape.ArrowDown,
        StartShapeColor = Color.Red,

        EndShape = GanttBarEndShape.ArrowUp,
        EndShapeColor = Color.Yellow,

        LeftField = Field.TaskResourceNames,
        RightField = Field.TaskName,
        TopField = Field.TaskStart,
        BottomField = Field.TaskFinish,
        InsideField = Field.TaskDuration
    };

    return style;
}
```

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

### See Also

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


