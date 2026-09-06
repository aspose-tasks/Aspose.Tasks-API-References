---
title: "SaveOptions.View"
second_title: "Aspose.Tasks for .NET API 参考"
description: "SaveOptions 属性。获取或设置要渲染的视图列列表 GanttChartColumn。如果未设置，则仅渲染任务 ID、任务名称、开始和结束。如果同时设置了 View 和 ViewSettings 属性，View 的列会覆盖 ViewSettings 的列。"
type: docs
weight: 230
url: /zh/net/aspose.tasks.saving/saveoptions/view/
---
## SaveOptions.View property

获取或设置要渲染的视图列列表 ([`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/))。如果未设置，则仅渲染任务 ID、任务名称、开始和结束。如果同时设置了 View 和 [`ViewSettings`](../viewsettings/) 属性，View 的列会覆盖 ViewSettings 的列。

```csharp
public ProjectView View { get; set; }
```

## 示例

展示如何在导出项目时添加要导出的视图列。

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
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


