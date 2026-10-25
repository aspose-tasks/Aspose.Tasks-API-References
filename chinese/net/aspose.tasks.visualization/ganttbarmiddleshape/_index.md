---
title: "枚举 GanttBarMiddleShape"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.GanttBarMiddleShape 枚举。指定条形的中间形状"
type: docs
weight: 3050
url: /zh/net/aspose.tasks.visualization/ganttbarmiddleshape/
---
## GanttBarMiddleShape enumeration

指定条形的中间形状。

```csharp
public enum GanttBarMiddleShape
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| LineBottom | `7` | 指示底部对齐的线形。 |
| LineMiddle | `6` | 指示居中对齐的线形。 |
| LineTop | `5` | 指示顶部对齐的线形。 |
| None | `0` | 表示空形状。 |
| RectangleBar | `1` | 表示全高矩形条形形状。 |
| RectangleBottom | `4` | 表示底部对齐的半高矩形条形形状。 |
| RectangleMiddle | `3` | 表示居中对齐的三分之一高矩形条形形状。 |
| RectangleTop | `2` | 指示顶部对齐的半高矩形条形形状。 |

## 示例

展示如何设置甘特图项目视图的自定义条样式。

```csharp
public void ImplementCustomBarStyle()
{
    try
    {
        var project = new Project(DataDir + "Blank2010.mpp");
        project.RootTask.Children.Add("Task");

        var view = (GanttChartView)project.DefaultView;
        var custom = GetCustomBarStyle();

        // 将自定义条样式添加到项目视图的自定义条集合中
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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


