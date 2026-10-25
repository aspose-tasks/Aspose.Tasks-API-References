---
title: "Spreadsheet2003SaveOptions.ResourceView"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Spreadsheet2003SaveOptions 属性。获取或设置要呈现的资源视图列列表 ResourceViewColumn"
type: docs
weight: 30
url: /zh/net/aspose.tasks.saving/spreadsheet2003saveoptions/resourceview/
---
## Spreadsheet2003SaveOptions.ResourceView property

获取或设置要呈现的资源视图列列表（[`ResourceViewColumn`](../../../aspose.tasks.visualization/resourceviewcolumn/)）。

```csharp
public ProjectView ResourceView { get; set; }
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

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [Spreadsheet2003SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../spreadsheet2003saveoptions/)
* assembly [Aspose.Tasks](../../../)


