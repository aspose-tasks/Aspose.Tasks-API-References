---
title: "类 TaskTextStyleEventArgs"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.TaskTextStyleEventArgs 类。此类表示与表格单元格内容渲染相关的数据集"
type: docs
weight: 3390
url: /zh/net/aspose.tasks.visualization/tasktextstyleeventargs/
---
## TaskTextStyleEventArgs class

此类表示与表格单元格内容渲染相关的数据集。

```csharp
public class TaskTextStyleEventArgs
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [CellTextStyle](../../aspose.tasks.visualization/tasktextstyleeventargs/celltextstyle/) { get; set; } | 获取或设置用于绘制单元格内容的 TextStyle。此对象可用于自定义表格单元格的外观。 |
| [Column](../../aspose.tasks.visualization/tasktextstyleeventargs/column/) { get; } | 获取当前渲染单元格所属的 [`ViewColumn`](../viewcolumn/)。 |
| [Task](../../aspose.tasks.visualization/tasktextstyleeventargs/task/) { get; } | 获取对应于当前渲染行的 [`Task`](./task/)。 |

## 示例

展示如何添加要导出的视图列。

```csharp
public void WorkWithViewColumn()
{
    var project = new Project(DataDir + "Project2.mpp");

    var options = new PdfSaveOptions();
    var columns = new List<ViewColumn>
    {
        new ResourceViewColumn(100, Field.ResourceName),
        new ResourceViewColumn(100, Field.ResourceActualWork),
        new ResourceViewColumn(100, Field.ResourceCost)
    };

    columns[0].TextStyleModificationCallback = new MyTextStyleCallback();

    // 遍历列
    foreach (var column in columns)
    {
        Console.WriteLine("Column Name: " + column.Name);
        Console.WriteLine("Column Field: " + column.Field);
        Console.WriteLine("Column Width: " + column.Width);
        Console.WriteLine("Column Callback: " + column.TextStyleModificationCallback);
        Console.WriteLine();
    }

    options.View = new ProjectView(columns);
    options.PresentationFormat = PresentationFormat.ResourceUsage;

    project.Save(OutDir + "WorkWithViewColumn_out.pdf", options);
}

private class MyTextStyleCallback : ITextStyleModificationCallback
{
    /// <summary>
    /// 在以下视图中，对任务行的表格单元格进行渲染之前调用的方法：
    /// 'Gantt Chart'、'Task Sheet'、'Task Usage'。
    /// </summary>
    /// <param name=\"args\">The <see cref=\"T:Aspose.Tasks.Visualization.TaskTextStyleEventArgs\" /> 对象。</param>
    public void BeforeTaskTextStyleApplied(TaskTextStyleEventArgs args)
    {
        if (args.Task.Get(Tsk.Uid) % 2 == 0)
        {
            args.CellTextStyle.BackgroundColor = 
                args.Column.StringAlignment == HorizontalStringAlignment.Center 
                ? Color.Cyan : Color.Red;
            args.CellTextStyle.BackgroundPattern = BackgroundPattern.SolidFill;
        }
        else
        {
            args.CellTextStyle.Color = Color.DarkGreen;
        }
    }
}
```

### 另见

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


