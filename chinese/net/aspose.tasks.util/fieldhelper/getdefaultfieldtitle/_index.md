---
title: "FieldHelper.GetDefaultFieldTitle"
second_title: "Aspose.Tasks for .NET API 参考"
description: "FieldHelper 方法。 返回特定字段的默认标题"
type: docs
weight: 10
url: /zh/net/aspose.tasks.util/fieldhelper/getdefaultfieldtitle/
---
## FieldHelper.GetDefaultFieldTitle method

返回特定字段的默认标题。

```csharp
public static string GetDefaultFieldTitle(Field field)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 字段 | 字段 | 用于获取默认标题的字段。 |

### 返回值

如果该字段可以在 MS Project 的视图中显示，则为特定字段的默认标题，否则为 null。

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

* enum [Field](../../../aspose.tasks/field/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)


