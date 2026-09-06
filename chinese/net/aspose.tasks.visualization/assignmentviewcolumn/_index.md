---
title: "类 AssignmentViewColumn"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.AssignmentViewColumn 类。项目视图类"
type: docs
weight: 2930
url: /zh/net/aspose.tasks.visualization/assignmentviewcolumn/
---
## AssignmentViewColumn class

项目视图类。

```csharp
public class AssignmentViewColumn : ViewColumn
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [AssignmentViewColumn](assignmentviewcolumn/)(string, int, AssignmentToColumnTextConverter) | 初始化 AssignmentViewColumn 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/assignmentviewcolumn/field/) { get; set; } | 列字段。[`Field`](./field/)。 |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | 获取列名。 |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | 获取或设置文本的对齐方式（可以是 [`HorizontalStringAlignment`](../horizontalstringalignment/) 枚举的其中一个值）。 |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | 获取或设置回调，可用于自定义列单元格的外观。 |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | 获取列宽。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/assignmentviewcolumn/getcolumntext/)(ResourceAssignment) | 将当前资源分配转换为列文本。 |

## 示例

展示如何为分配视图添加列。

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new Spreadsheet2003SaveOptions();

var column = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(column);

foreach (var assignment in project.ResourceAssignments)
{
    foreach (var col in options.AssignmentView.Columns)
    {
        var assnCol = (AssignmentViewColumn)col;
        Console.WriteLine("Column Field: " + assnCol.Field);
        Console.WriteLine("Column Text ( converted ): " + assnCol.GetColumnText(assignment));
        Console.WriteLine();
    }
}

project.Save(OutDir + "UsingSpreadsheet2003SaveOptions_out.xml", options);
```

### 另见

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


