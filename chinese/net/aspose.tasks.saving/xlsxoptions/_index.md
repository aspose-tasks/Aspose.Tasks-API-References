---
title: "类 XlsxOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Saving.XlsxOptions 类。允许在将项目页面渲染为 XLSX 时指定其他选项"
type: docs
weight: 2270
url: /zh/net/aspose.tasks.saving/xlsxoptions/
---
## XlsxOptions class

允许在将项目页面渲染为 XLSX 时指定其他选项。

```csharp
public class XlsxOptions : SimpleSaveOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [XlsxOptions](xlsxoptions/)() | 初始化 `XlsxOptions` 类的新实例，可用于将项目保存为 XLSX 格式。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [AssignmentView](../../aspose.tasks.saving/xlsxoptions/assignmentview/) { get; set; } | 获取或设置要呈现的分配视图列列表（[`AssignmentViewColumn`](../../aspose.tasks.visualization/assignmentviewcolumn/)）。 |
| [Encoding](../../aspose.tasks.saving/xlsxoptions/encoding/) { get; set; } | 获取或设置生成的 XLSX 文件的编码。默认值为 UTF8。 |
| [ResourceView](../../aspose.tasks.saving/xlsxoptions/resourceview/) { get; set; } | 获取或设置要呈现的资源视图列列表（[`ResourceViewColumn`](../../aspose.tasks.visualization/resourceviewcolumn/)）。 |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | 获取或设置如果使用此保存选项对象，文档将被保存的格式。 |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | 获取或设置用于在甘特图和任务表图上排序任务的比较器。 |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | 获取或设置用于过滤在甘特图、任务表和任务使用图上渲染的任务的条件。 |
| [View](../../aspose.tasks.saving/xlsxoptions/view/) { get; set; } | 获取或设置要保存为 XLSX 格式的视图列列表（[`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)）。如果未设置，则保存默认列。 |

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

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


