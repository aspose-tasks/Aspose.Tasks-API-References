---
title: "SaveOptions.LegendItems"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "SaveOptions プロパティ。ページ凡例にレンダリングすべきバーを定義する PageLegendItem の配列を取得または設定します。null の場合はデフォルト項目がレンダリングされます"
type: docs
weight: 90
url: /ja/net/aspose.tasks.saving/saveoptions/legenditems/
---
## SaveOptions.LegendItems property

ページ凡例にレンダリングすべきバーを定義する PageLegendItem の配列を取得または設定します。null の場合、デフォルト項目がレンダリングされます。

```csharp
public PageLegendItem[] LegendItems { get; set; }
```

## 備考

Gantt チャートビューがレンダリングされる場合にのみ適用されます。

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

* class [PageLegendItem](../../../aspose.tasks.visualization/pagelegenditem/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


