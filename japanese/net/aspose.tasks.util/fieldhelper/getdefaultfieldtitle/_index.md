---
title: "FieldHelper.GetDefaultFieldTitle"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "FieldHelper メソッド。特定のフィールドのデフォルトタイトルを返します。"
type: docs
weight: 10
url: /ja/net/aspose.tasks.util/fieldhelper/getdefaultfieldtitle/
---
## FieldHelper.GetDefaultFieldTitle method

特定のフィールドのデフォルトタイトルを返します。

```csharp
public static string GetDefaultFieldTitle(Field field)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| フィールド | フィールド | デフォルトタイトルを取得するフィールド。 |

### 戻り値

フィールドが MS Project のビューに表示できる場合は特定のフィールドのデフォルトタイトルを返し、表示できない場合は null を返します。

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

* enum [Field](../../../aspose.tasks/field/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)


