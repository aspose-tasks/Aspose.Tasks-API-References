---
title: "委托 AssignmentToColumnTextConverter"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ResourceAssignment 数据到列的字符串转换器"
type: docs
weight: 2920
url: /zh/net/aspose.tasks.visualization/assignmenttocolumntextconverter/
---
## AssignmentToColumnTextConverter delegate

ResourceAssignment 数据到列字符串的转换器。

```csharp
public delegate string AssignmentToColumnTextConverter(ResourceAssignment assignment);
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 分配 | ResourceAssignment | 要转换的分配。 |

### 返回值

列的字符串数据。

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

* class [ResourceAssignment](../../aspose.tasks/resourceassignment/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


