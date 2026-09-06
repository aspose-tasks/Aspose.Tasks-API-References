---
title: "GanttChartView.CustomBarStyles"
second_title: "Aspose.Tasks for .NET API 参考"
description: "GanttChartView 属性。获取 Gantt Chart 视图的自定义任务特定条形样式列表。GanttBarStyle"
type: docs
weight: 70
url: /zh/net/aspose.tasks/ganttchartview/custombarstyles/
---
## GanttChartView.CustomBarStyles property

获取 Gantt Chart 视图的自定义任务特定条形样式列表。[`GanttBarStyle`](../../../aspose.tasks.visualization/ganttbarstyle/)。

```csharp
public List<GanttBarStyle> CustomBarStyles { get; }
```

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

* class [GanttBarStyle](../../../aspose.tasks.visualization/ganttbarstyle/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


