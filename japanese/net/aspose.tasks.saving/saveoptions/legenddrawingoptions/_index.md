---
title: "SaveOptions.LegendDrawingOptions"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "SaveOptions プロパティ。凡例の描画方法を定義する値を取得または設定します。デフォルト値は LegendDrawingOptions.OnEveryPage です"
type: docs
weight: 80
url: /ja/net/aspose.tasks.saving/saveoptions/legenddrawingoptions/
---
## SaveOptions.LegendDrawingOptions property

凡例の描画方法を定義する値を取得または設定します。デフォルト値は LegendDrawingOptions.OnEveryPage です。

```csharp
public LegendDrawingOptions LegendDrawingOptions { get; set; }
```

## 備考

Gantt チャートビューがレンダリングされる場合にのみ適用されます。

## 例

最後のページに凡例を印刷する方法を示します

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // ビューから凡例描画オプションを取得します
    LegendDrawingOptions = LegendDrawingOptions.AfterLastPage
};

project.Save(OutDir + "LegendOnSeparatePage_out.pdf", options);
```

ページ凡例を非表示にする方法を示します。

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // 凡例を非表示にするには LegendDrawingOptions.NoLegend を指定します
    LegendDrawingOptions = LegendDrawingOptions.NoLegend
};

project.Save(OutDir + "HideLegendsDuringSave_out.pdf", options);
```

LegendDrawingOptions.DefinedInView オプションの使用方法を示します。

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var view = project.Views.GetByName("&Gantt Chart");

Console.WriteLine("LegendOn option defined in view '{0}': {1}", view.Name, view.PageInfo.Legend.LegendOn);

SaveOptions options = new PdfSaveOptions
{
    // ビューから凡例描画オプションを取得します
    LegendDrawingOptions = LegendDrawingOptions.DefinedInView,
    ViewSettings = view
};

project.Save(OutDir + "Legend_DefinedInView.pdf", options);
```

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

* enum [LegendDrawingOptions](../../legenddrawingoptions/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


