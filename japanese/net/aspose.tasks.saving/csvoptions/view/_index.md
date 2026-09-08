---
title: "CsvOptions.View"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "CsvOptions プロパティ。XLSX 形式で保存するためのビュー列 GanttChartColumn のリストを取得または設定します。設定されていない場合、デフォルトの列が保存されます"
type: docs
weight: 60
url: /ja/net/aspose.tasks.saving/csvoptions/view/
---
## CsvOptions.View property

XLSX 形式で保存するためのビュー列（[`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/)）のリストを取得または設定します。設定されていない場合、デフォルトの列が保存されます。

```csharp
public ProjectView View { get; set; }
```

## 例

デフォルトのガントチャートの列を取得するために &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt; の使用方法を示し、

```csharp
// それらを CSV ファイルに保存します。
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

### 関連項目

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


