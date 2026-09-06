---
title: "类 GanttChartColumn"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.GanttChartColumn 类。项目视图类"
type: docs
weight: 3090
url: /zh/net/aspose.tasks.visualization/ganttchartcolumn/
---
## GanttChartColumn class

项目视图类

```csharp
public sealed class GanttChartColumn : ViewColumn
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [GanttChartColumn](ganttchartcolumn/#constructor)(int, Field) | 初始化 GanttChartColumn 类的新实例。 |
| [GanttChartColumn](ganttchartcolumn/#constructor_1)(string, int, Field) | 初始化 GanttChartColumn 类的新实例。 |
| [GanttChartColumn](ganttchartcolumn/#constructor_2)(string, int, TaskToColumnTextConverter) | 初始化 GanttChartColumn 类的新实例。 |
| [GanttChartColumn](ganttchartcolumn/#constructor_3)(string, int, TaskToColumnTextConverter, Field) | 初始化 GanttChartColumn 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/ganttchartcolumn/field/) { get; set; } | 列字段。[`Field`](./field/)。 |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | 获取列名。 |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | 获取或设置文本的对齐方式（可以是 [`HorizontalStringAlignment`](../horizontalstringalignment/) 枚举的其中一个值）。 |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | 获取或设置回调，可用于自定义列单元格的外观。 |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | 获取列宽。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/ganttchartcolumn/getcolumntext/)(Task) | 将当前任务转换为列文本。 |

## 示例

展示如何添加要导出的甘特图视图列。

```csharp
var project = new Project(DataDir + "Project2.mpp");
var task = project.RootTask.Children.GetById(1);

var columns = new List<ViewColumn>
{
    new GanttChartColumn(20, Field.TaskUniqueID),
    new GanttChartColumn("Name", 150, Field.TaskName),
    new GanttChartColumn("Start", 100, Field.TaskStart),
    new GanttChartColumn("End", 100, Field.TaskFinish),
    new GanttChartColumn("R-Initials", 100, Field.TaskResourceInitials),
    new GanttChartColumn("R-Names", 100, Field.TaskResourceNames),
    new GanttChartColumn("Work", 50, Field.TaskWork),
    new GanttChartColumn(
        "Cost", 
        80,
        delegate(Task t)
        {
            return t.Get(Tsk.Cost).ToString(CultureInfo.InvariantCulture);
        }),
    new GanttChartColumn(
        "Actual Cost", 
        80,
        delegate(Task t)
        {
            return t.Get(Tsk.ActualCost).ToString(CultureInfo.InvariantCulture);
        },
        Field.TaskActualCost)
};

// 遍历列
foreach (var column in columns)
{
    var col = (GanttChartColumn)column;
    Console.WriteLine("Column Name: " + col.Name);
    Console.WriteLine("Column Field: " + col.Field);
    Console.WriteLine("Column Text: " + col.GetColumnText(task));
    Console.WriteLine();
}

var options = new CsvOptions
{
    View = new ProjectView(columns)
};

project.Save(OutDir + "WorkWithGanttChartColumn_out.csv", options);
```

### 另见

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


