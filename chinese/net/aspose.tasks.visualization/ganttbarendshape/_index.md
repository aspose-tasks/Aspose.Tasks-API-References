---
title: "枚举 GanttBarEndShape"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.GanttBarEndShape 枚举。表示栏和进度线中进度点的结束形状"
type: docs
weight: 3030
url: /zh/net/aspose.tasks.visualization/ganttbarendshape/
---
## GanttBarEndShape enumeration

表示条形和进度线中的结束形状以及进度点。

```csharp
public enum GanttBarEndShape
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| ArrowDown | `14` | 指示向下箭头的甘特栏结束形状。 |
| ArrowUp | `8` | 指示向上箭头的甘特栏结束形状。 |
| CaretDownTop | `9` | 指示位于栏上半部的向下插入符号的甘特栏结束形状。 |
| CaretUpBottom | `10` | 指示位于栏下半部的向上插入符号的甘特栏结束形状。 |
| Circle | `19` | 指示圆形的甘特栏结束形状。 |
| CircleArrowDown | `18` | 指示带圆圈的向下箭头的甘特栏结束形状。 |
| CircleArrowUp | `17` | 指示带圆圈的向上箭头的甘特栏结束形状。 |
| CircleDiamond | `13` | 指示带圆圈的菱形的甘特栏结束形状。 |
| CircleTriangleDown | `16` | 指示带圆圈的向下三角形的甘特栏结束形状。 |
| CircleTriangleUp | `15` | 指示带圆圈的向上三角形的甘特栏结束形状。 |
| Diamond | `3` | 指示菱形的甘特栏结束形状。 |
| HouseDown | `2` | 指示倒置房屋形状的甘特栏结束形状。 |
| HouseUp | `1` | 指示房屋形状的甘特栏结束形状。 |
| LeftBracket | `21` | 指示左括号的甘特栏结束形状。 |
| LeftFade | `23` | 指示左侧淡化的甘特栏结束形状。 |
| LineShape | `11` | 指示线形的甘特栏结束形状。 |
| NoBarEndShape | `0` | 指示无形状的甘特栏结束形状。 |
| RightBracket | `22` | 指示右括号的甘特栏结束形状。 |
| RightFade | `24` | 指示右侧淡化的甘特栏结束形状。 |
| Square | `12` | 指示方形的甘特栏结束形状。 |
| Star | `20` | 指示星形的甘特栏结束形状。 |
| TriangleDown | `5` | 指示向下三角形的甘特栏结束形状。 |
| TriangleLeft | `7` | 指示左指向的三角形甘特条结束形状。 |
| TriangleRight | `6` | 指示右指向的三角形甘特条结束形状。 |
| TriangleUp | `4` | 指示带圆圈的向上三角形的甘特栏结束形状。 |

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


