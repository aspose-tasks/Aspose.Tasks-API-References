---
title: "PageSettings.IsPortrait"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PageSettings 属性。获取或设置一个值，指示页面方向是否为纵向；如果页面方向为横向则返回 false"
type: docs
weight: 40
url: /zh/net/aspose.tasks.visualization/pagesettings/isportrait/
---
## PageSettings.IsPortrait property

获取或设置一个值，指示页面方向是否为纵向；如果页面方向为横向，则返回 false。

```csharp
public bool IsPortrait { get; set; }
```

## 备注

在渲染期间适用，当 SaveOptions.PageSize == Visualization.PageSize.DefinedInView 时。

## 示例

展示如何使用 &lt;see cref=\"Aspose.Tasks.Visualization.PageSettings\" /&gt;。

```csharp
var project = new Project(DataDir + "Project2.mpp");

// 获取设置
var settings = project.DefaultView.PageInfo.PageSettings;
// 让我们调优一些属性
// 设置一个值，指示页面方向是否为纵向；如果页面方向为横向则返回 false。
settings.IsPortrait = true;
// 设置要打印的水平页数。
settings.PagesInWidth = 5;
// 设置要打印的垂直页数。
settings.PagesInHeight = 7;
// 设置用于调整打印的正常大小的百分比。
settings.PercentOfNormalSize = 200;
// 设置纸张大小。可以是 <see cref=\"T:Aspose.Tasks.Visualization.PrinterPaperSize\" /> 枚举的其中一个值。
settings.PaperSize = PrinterPaperSize.PaperB4;
// 设置打印的起始页码。
settings.FirstPageNumber = 3;

SimpleSaveOptions options = new MPPSaveOptions
{
    WriteViewData = true
};

project.Save(OutDir + "TestCanWritePageSettings.mpp", options);
```

展示如何使用 View 设置或使用 SaveOptions 指定页面大小和方向。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

saveOptions.PageSize = PageSize.DefinedInView;

// 在这种情况下，页面大小和方向取自 view.PageInfo.PageSettings.PaperSize 和 view.PageInfo.PageSettings.IsPortrait 属性。
project.Save(OutDir + "WorkWithIsPortrait_out1.pdf", saveOptions);

saveOptions.PageSize = PageSize.A4;
saveOptions.IsPortrait = true;

// 在这种情况下，页面大小和方向取自 SaveOptions 的属性。
project.Save(OutDir + "WorkWithIsPortrait_out2.pdf", saveOptions);

saveOptions.CustomPageSize = new SizeF(400, 600);

// 在这种情况下，页面大小取自 SaveOptions.CustomPageSize。IsPortrait 属性不予考虑。
project.Save(OutDir + "WorkWithIsPortrait_out3.pdf", saveOptions);
```

### 另见

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


