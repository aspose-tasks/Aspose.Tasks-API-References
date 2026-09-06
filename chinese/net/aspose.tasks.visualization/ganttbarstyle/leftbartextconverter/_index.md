---
title: "GanttBarStyle.LeftBarTextConverter"
second_title: "Aspose.Tasks for .NET API 参考"
description: "GanttBarStyle 属性。获取或设置用户定义的转换器，以获取在任务栏左侧渲染的文本。覆盖 LeftField 属性的值。不会持久化到 MPP 格式"
type: docs
weight: 100
url: /zh/net/aspose.tasks.visualization/ganttbarstyle/leftbartextconverter/
---
## GanttBarStyle.LeftBarTextConverter property

获取或设置用户定义的转换器，以获取在任务栏左侧渲染的文本。覆盖 [`LeftField`](../leftfield/) 属性的值。不会持久化到 MPP 格式。

```csharp
public TaskBarTextConverter LeftBarTextConverter { get; set; }
```

## 示例

展示如何使用甘特图视图的自定义条样式。

```csharp
var project = new Project(DataDir + "Project2.mpp");

var ganttChartView = (GanttChartView)project.Views.First(v => v.Name == "Gantt &Chart");
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.ViewSettings = ganttChartView;

// 条样式可以是任务特定的（位于 GanttChartView.CustomBarStyles）
// 或类别特定的（位于 GanttChartView.BarStyles）
foreach (GanttBarStyle ganttBarStyle in ganttChartView.CustomBarStyles)
{
    if (ganttBarStyle.ShowForTaskUid != 4)
    {
        continue;
    }

    // 出于演示目的，我们正在修改唯一 ID 为 4 的任务的样式
    // 这里我们将字段 (TaskName) 设置为在任务条的左侧渲染。
    ganttBarStyle.LeftField = Field.TaskName;
    // 这里我们设置自定义转换器，以控制应在任务条内部渲染的文本。
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

    // 出于演示目的，我们正在修改适用于里程碑任务的样式。

    ganttBarStyle.StartShape = GanttBarEndShape.Diamond;
    ganttBarStyle.RightField = Field.TaskActualFinish;
    ganttBarStyle.TopBarTextConverter = task => task.Get(Tsk.ActualStart).Day.ToString();
}

project.Save(OutDir + "WorkWithGanttChartViewBarStyles_out.pdf", saveOptions);
```

### 另见

* delegate [TaskBarTextConverter](../../taskbartextconverter/)
* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


