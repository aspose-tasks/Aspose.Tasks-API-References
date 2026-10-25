---
title: "类 ViewColumn"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.ViewColumn 类。表示项目视图中的一列"
type: docs
weight: 3470
url: /zh/net/aspose.tasks.visualization/viewcolumn/
---
## ViewColumn class

表示项目视图中的一列。

```csharp
public abstract class ViewColumn
```

## 属性

| 名称 | 描述 |
| --- | --- |
| abstract [Field](../../aspose.tasks.visualization/viewcolumn/field/) { get; set; } | 获取或设置列字段。[`Field`](./field/)。 |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | 获取列名。 |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | 获取或设置文本的对齐方式（可以是 [`HorizontalStringAlignment`](../horizontalstringalignment/) 枚举的其中一个值）。 |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | 获取或设置回调，可用于自定义列单元格的外观。 |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | 获取列宽。 |

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


