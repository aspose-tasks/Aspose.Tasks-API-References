---
title: "Class PageLegendItem"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "Aspose.Tasks.Visualization.PageLegendItem class. ガントチャートのページ凡例項目を表します"
type: docs
weight: 3220
url: /ja/net/aspose.tasks.visualization/pagelegenditem/
---
## PageLegendItem class

ガントチャートのページ凡例項目を表します。

```csharp
public sealed class PageLegendItem
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [PageLegendItem](pagelegenditem/)(BarItemType, string) | `PageLegendItem` クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [ItemType](../../aspose.tasks.visualization/pagelegenditem/itemtype/) { get; } | 項目の型を取得します。 |
| [Title](../../aspose.tasks.visualization/pagelegenditem/title/) { get; } | 項目のテキストラベルを取得します。 |

## 例

ガントチャートのページ凡例でタスクバーをカスタマイズする方法を示します。

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.StartDate = project.StartDate;
pdfSaveOptions.EndDate = project.FinishDate;
pdfSaveOptions.PageSize = PageSize.A4;
pdfSaveOptions.LegendDrawingOptions = LegendDrawingOptions.OnEveryPage;
pdfSaveOptions.ViewSettings = project.Views.GetByName("&Gantt Chart");

pdfSaveOptions.LegendItems = new PageLegendItem[]
{
    new PageLegendItem(BarItemType.Task, "Task"),
    new PageLegendItem(BarItemType.ExternalMilestone, "External Milestone"),
    new PageLegendItem(BarItemType.SummaryRollup, "Summary Rollup"),
    new PageLegendItem(BarItemType.InactiveTask, "Inactive Task"),
    new PageLegendItem(BarItemType.ManualSummary, "Manual Summary")
};

project.Save(OutDir + "CustomizePageLegendItems_out.pdf", pdfSaveOptions);
```

### 関連項目

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


