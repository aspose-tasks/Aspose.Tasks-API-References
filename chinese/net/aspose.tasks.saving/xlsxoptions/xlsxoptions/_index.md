---
title: "XlsxOptions.XlsxOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "XlsxOptions 构造函数。初始化一个可用于以 XLSX 格式保存项目的 XlsxOptions 类的新实例。"
type: docs
weight: 10
url: /zh/net/aspose.tasks.saving/xlsxoptions/xlsxoptions/
---
## XlsxOptions constructor

初始化一个可用于以 XLSX 格式保存项目的 [`XlsxOptions`](../) 类的新实例。

```csharp
public XlsxOptions()
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

* class [XlsxOptions](../)
* namespace [Aspose.Tasks.Saving](../../xlsxoptions/)
* assembly [Aspose.Tasks](../../../)


