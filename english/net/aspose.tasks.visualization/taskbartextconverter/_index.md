---
title: Delegate TaskBarTextConverter
second_title: Aspose.Tasks for .NET API Reference
description: Custom converter of tasks data to bar text
type: docs
weight: 3300
url: /net/aspose.tasks.visualization/taskbartextconverter/
---
## TaskBarTextConverter delegate

Custom converter of task's data to bar text.

```csharp
public delegate string TaskBarTextConverter(Task task);
```

| Parameter | Type | Description |
| --- | --- | --- |
| task | Task | Task for which task bar's text will be rendered. |

### Return Value

Text to render for a bar corresponding to the specified task.

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

### See Also

* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


