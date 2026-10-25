---
title: "类 Spreadsheet2003SaveOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Saving.Spreadsheet2003SaveOptions 类。允许在将项目页面呈现为 Spreadsheet2003 时指定其他选项。"
type: docs
weight: 2220
url: /zh/net/aspose.tasks.saving/spreadsheet2003saveoptions/
---
## Spreadsheet2003SaveOptions class

允许在将项目页面渲染为 Spreadsheet2003 时指定附加选项。

```csharp
public class Spreadsheet2003SaveOptions : SimpleSaveOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [Spreadsheet2003SaveOptions](spreadsheet2003saveoptions/)() | 初始化 `Spreadsheet2003SaveOptions` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [AssignmentView](../../aspose.tasks.saving/spreadsheet2003saveoptions/assignmentview/) { get; set; } | 获取或设置要呈现的分配视图列列表（[`AssignmentViewColumn`](../../aspose.tasks.visualization/assignmentviewcolumn/)）。 |
| [ResourceView](../../aspose.tasks.saving/spreadsheet2003saveoptions/resourceview/) { get; set; } | 获取或设置要呈现的资源视图列列表（[`ResourceViewColumn`](../../aspose.tasks.visualization/resourceviewcolumn/)）。 |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | 获取或设置如果使用此保存选项对象，文档将被保存的格式。 |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | 获取或设置用于在甘特图和任务表图上排序任务的比较器。 |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | 获取或设置用于过滤在甘特图、任务表和任务使用图上渲染的任务的条件。 |
| [View](../../aspose.tasks.saving/spreadsheet2003saveoptions/view/) { get; set; } | 获取或设置要保存的视图列列表（[`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)）。如果未设置，则保存默认列。 |

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

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


