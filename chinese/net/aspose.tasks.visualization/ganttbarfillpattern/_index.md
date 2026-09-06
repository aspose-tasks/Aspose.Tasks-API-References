---
title: "枚举 GanttBarFillPattern"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.GanttBarFillPattern 枚举。形状的填充模式"
type: docs
weight: 3040
url: /zh/net/aspose.tasks.visualization/ganttbarfillpattern/
---
## GanttBarFillPattern enumeration

形状的填充图案。

```csharp
public enum GanttBarFillPattern
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Hollow | `0` | 空心模式。 |
| SolidFill | `1` | 实心填充模式。 |
| LightFill | `2` | 浅色填充模式。 |
| MediumFill | `3` | 中等填充模式。 |
| DarkFill | `4` | 深色填充模式。 |
| DiagonalLeft | `5` | 左对角线图案（从左上到右下）。 |
| DiagonalRight | `6` | 右对角线图案（从右上到左下）。 |
| DiagonalCross | `7` | 对角交叉图案。 |
| LineVertical | `8` | 垂直线图案。 |
| LineHorizontal | `9` | 水平线图案。 |
| LineCross | `10` | 交叉线图案。 |
| SolidFillWithDashedBorder | `11` | 实线带虚线边框的图案。 |

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

### 另见

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


