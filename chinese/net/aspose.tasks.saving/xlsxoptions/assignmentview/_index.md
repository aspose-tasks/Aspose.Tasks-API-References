---
title: "XlsxOptions.AssignmentView"
second_title: "Aspose.Tasks for .NET API 参考"
description: "XlsxOptions 属性。获取或设置用于呈现 AssignmentViewColumn 的任务视图列列表。"
type: docs
weight: 20
url: /zh/net/aspose.tasks.saving/xlsxoptions/assignmentview/
---
## XlsxOptions.AssignmentView property

获取或设置要渲染的任务视图列列表（[`AssignmentViewColumn`](../../../aspose.tasks.visualization/assignmentviewcolumn/)）。

```csharp
public ProjectView AssignmentView { get; set; }
```

## 示例

展示如何通过使用 &lt;see cref="P:Aspose.Tasks.Saving.XlsxOptions"&gt;Days&lt;/see&gt; 选项将项目保存为 XLSX 文件。

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new XlsxOptions();

// 添加所需的甘特图列
var col = new GanttChartColumn("WBS", 100, delegate(Task task) { return task.Get(Tsk.WBS); });
options.View.Columns.Add(col);

// 添加所需的资源视图列
var rscCol = new ResourceViewColumn("Cost center", 100, delegate(Resource resource) { return resource.Get(Rsc.CostCenter); });
options.ResourceView.Columns.Add(rscCol);

// 添加所需的分配视图列
var assnCol = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(assnCol);

// 设置编码
options.Encoding = Encoding.Unicode;

project.Save(OutDir + "UsingXlsxOptions_out.xlsx", options);
```

### 另见

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [XlsxOptions](../)
* namespace [Aspose.Tasks.Saving](../../xlsxoptions/)
* assembly [Aspose.Tasks](../../../)


