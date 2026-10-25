---
title: "AssignmentViewColumn.GetColumnText"
second_title: "Aspose.Tasks for .NET API 参考"
description: "AssignmentViewColumn 方法。将当前资源分配转换为列文本"
type: docs
weight: 30
url: /zh/net/aspose.tasks.visualization/assignmentviewcolumn/getcolumntext/
---
## AssignmentViewColumn.GetColumnText method

将当前资源分配转换为列文本。

```csharp
public string GetColumnText(ResourceAssignment assignment)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 分配 | ResourceAssignment | 当前分配。 |

### 返回值

列文本。

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

* class [ResourceAssignment](../../../aspose.tasks/resourceassignment/)
* class [AssignmentViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../assignmentviewcolumn/)
* assembly [Aspose.Tasks](../../../)


