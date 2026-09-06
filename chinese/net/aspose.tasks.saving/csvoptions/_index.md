---
title: "类 CsvOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Saving.CsvOptions 类。允许在将项目保存为 CSV 时指定附加选项"
type: docs
weight: 1980
url: /zh/net/aspose.tasks.saving/csvoptions/
---
## CsvOptions class

允许在将项目保存为 CSV 时指定附加选项。

```csharp
public class CsvOptions : SimpleSaveOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [CsvOptions](csvoptions/)() | 初始化一个 `CsvOptions` 类的新实例，可用于以 CSV 格式保存项目。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [DataCategory](../../aspose.tasks.saving/csvoptions/datacategory/) { get; set; } | 获取或设置要保存的数据类别。 |
| [Encoding](../../aspose.tasks.saving/csvoptions/encoding/) { get; set; } | 获取或设置用于保存 CSV 的编码。 |
| [IncludeHeaders](../../aspose.tasks.saving/csvoptions/includeheaders/) { get; set; } | 获取或设置一个值，指示是否包含标题（默认值为 TRUE）。 |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | 获取或设置如果使用此保存选项对象，文档将被保存的格式。 |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | 获取或设置用于在甘特图和任务表图上排序任务的比较器。 |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | 获取或设置用于过滤在甘特图、任务表和任务使用图上渲染的任务的条件。 |
| [TextDelimiter](../../aspose.tasks.saving/csvoptions/textdelimiter/) { get; set; } | 获取或设置文本分隔符。 |
| [View](../../aspose.tasks.saving/csvoptions/view/) { get; set; } | 获取或设置要保存为 XLSX 格式的视图列列表（[`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)）。如果未设置，则保存默认列。 |

## 示例

展示如何使用 &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt; 将项目保存为 CSV 文件。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
var options = new CsvOptions
{
    DataCategory = DataCategory.Resources,
    TextDelimiter = CsvTextDelimiter.Semicolon,
    Encoding = Encoding.Unicode, IncludeHeaders = true
};

project.Save(OutDir + "WorkWithCsvOptions_out.csv", options);
```

展示如何使用 &lt;see cref="Aspose.Tasks.Saving.CsvOptions" /&gt; 获取默认甘特图的列并

```csharp
// 将它们保存为 CSV 文件。
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

CsvOptions options = new CsvOptions();
options.TextDelimiter = CsvTextDelimiter.Tab;

var view = project.DefaultView;
options.View = ProjectView.GetDefaultGanttChartView();
options.View.Columns.Clear();

foreach (var t in view.Table.TableFields)
{
    var columnTitle = string.IsNullOrEmpty(t.Title) ? FieldHelper.GetDefaultFieldTitle(t.Field) : t.Title;
    options.View.Columns.Add(new GanttChartColumn(columnTitle, 10, t.Field));
}

project.Save(OutDir + "CustomizeViewForCsvOptions_out.csv", options);
```

### 另见

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


