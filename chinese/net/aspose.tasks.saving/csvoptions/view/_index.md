---
title: "CsvOptions.View"
second_title: "Aspose.Tasks for .NET API 参考"
description: "CsvOptions 属性。获取或设置要保存为 XLSX 格式的视图列 GanttChartColumn 列表。如果未设置，则保存默认列"
type: docs
weight: 60
url: /zh/net/aspose.tasks.saving/csvoptions/view/
---
## CsvOptions.View property

获取或设置要保存为 XLSX 格式的视图列（[`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/)）列表。如果未设置，则保存默认列。

```csharp
public ProjectView View { get; set; }
```

## 示例

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

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


