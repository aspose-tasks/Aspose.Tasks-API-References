---
title: "Spreadsheet2003SaveOptions.Spreadsheet2003SaveOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Spreadsheet2003SaveOptions 构造函数。初始化 Spreadsheet2003SaveOptions 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks.saving/spreadsheet2003saveoptions/spreadsheet2003saveoptions/
---
## Spreadsheet2003SaveOptions constructor

初始化 [`Spreadsheet2003SaveOptions`](../) 类的新实例。

```csharp
public Spreadsheet2003SaveOptions()
```

## 示例

展示如何在导出项目为 Spreadsheet2003 格式时添加要导出的列。

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new Spreadsheet2003SaveOptions();
var ganttChartColumn = new GanttChartColumn("WBS", 100, delegate(Task task) { return task.Get(Tsk.WBS); });
options.View.Columns.Add(ganttChartColumn);

var resourceViewColumn = new ResourceViewColumn("Cost center", 100, delegate(Resource resource) { return resource.Get(Rsc.CostCenter); });
options.ResourceView.Columns.Add(resourceViewColumn);

var assignmentViewColumn = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(assignmentViewColumn);

project.Save(OutDir + "UsingSpreadsheet2003SaveOptions_out.xml", options);
```

### 另见

* class [Spreadsheet2003SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../spreadsheet2003saveoptions/)
* assembly [Aspose.Tasks](../../../)


