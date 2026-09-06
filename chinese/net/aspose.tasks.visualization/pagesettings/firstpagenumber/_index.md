---
title: "PageSettings.FirstPageNumber"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PageSettings 属性。获取或设置打印的起始页码"
type: docs
weight: 30
url: /zh/net/aspose.tasks.visualization/pagesettings/firstpagenumber/
---
## PageSettings.FirstPageNumber property

获取或设置打印的起始页码。

```csharp
public short FirstPageNumber { get; set; }
```

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

### 另见

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


