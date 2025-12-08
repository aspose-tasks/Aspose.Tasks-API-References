---
title: Enum GanttBarEndShape
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.GanttBarEndShape enum. Represents end shape in bars and progress points in progress lines
type: docs
weight: 2980
url: /net/aspose.tasks.visualization/ganttbarendshape/
---
## GanttBarEndShape enumeration

Represents end shape in bars and progress points in progress lines.

```csharp
public enum GanttBarEndShape
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| ArrowDown | `14` | Indicates Arrow pointing down Gantt bar end shape. |
| ArrowUp | `8` | Indicates Arrow pointing up Gantt bar end shape. |
| CaretDownTop | `9` | Indicates Caret pointing down on the top half of the bar Gantt bar end shape. |
| CaretUpBottom | `10` | Indicates Caret pointing up on the bottom half of the bar Gantt bar end shape. |
| Circle | `19` | Indicates Circle Gantt bar end shape. |
| CircleArrowDown | `18` | Indicates Circled arrow pointing down Gantt bar end shape. |
| CircleArrowUp | `17` | Indicates Circled arrow pointing up Gantt bar end shape. |
| CircleDiamond | `13` | Indicates Circled diamond Gantt bar end shape. |
| CircleTriangleDown | `16` | Indicates Circled triangle pointing down Gantt bar end shape. |
| CircleTriangleUp | `15` | Indicates Circled triangle pointing up Gantt bar end shape. |
| Diamond | `3` | Indicates Diamond Gantt bar end shape. |
| HouseDown | `2` | Indicates Upside-down house Gantt bar end shape. |
| HouseUp | `1` | Indicates House Gantt bar end shape. |
| LeftBracket | `21` | Indicates Left bracket Gantt bar end shape. |
| LeftFade | `23` | Indicates Left fade Gantt bar end shape. |
| LineShape | `11` | Indicates Line Gantt bar end shape. |
| NoBarEndShape | `0` | Indicates None Gantt bar end shape. |
| RightBracket | `22` | Indicates Right bracket Gantt bar end shape. |
| RightFade | `24` | Indicates Right fade Gantt bar end shape. |
| Square | `12` | Indicates Square Gantt bar end shape. |
| Star | `20` | Indicates Star Gantt bar end shape. |
| TriangleDown | `5` | Indicates Triangle pointing down Gantt bar end shape. |
| TriangleLeft | `7` | Indicates Triangle pointing left Gantt bar end shape. |
| TriangleRight | `6` | Indicates Triangle pointing right Gantt bar end shape. |
| TriangleUp | `4` | Indicates Circled triangle pointing up Gantt bar end shape. |

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


