---
title: "ITextStyleModificationCallback.BeforeTaskTextStyleApplied"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ITextStyleModificationCallback 方法。该方法在以下视图（甘特图、任务表、任务使用）中，在任务行的表格单元格渲染之前被调用"
type: docs
weight: 10
url: /zh/net/aspose.tasks.visualization/itextstylemodificationcallback/beforetasktextstyleapplied/
---
## ITextStyleModificationCallback.BeforeTaskTextStyleApplied method

在以下视图中，对任务行的表格单元格进行渲染之前调用的方法：'Gantt Chart'、'Task Sheet'、'Task Usage'。

```csharp
public void BeforeTaskTextStyleApplied(TaskTextStyleEventArgs args)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| args | TaskTextStyleEventArgs | [`TaskTextStyleEventArgs`](../../tasktextstyleeventargs/) 对象。 |

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

* class [TaskTextStyleEventArgs](../../tasktextstyleeventargs/)
* interface [ITextStyleModificationCallback](../)
* namespace [Aspose.Tasks.Visualization](../../itextstylemodificationcallback/)
* assembly [Aspose.Tasks](../../../)


