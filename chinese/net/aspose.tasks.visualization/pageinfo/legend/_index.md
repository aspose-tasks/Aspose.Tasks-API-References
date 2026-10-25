---
title: "PageInfo.Legend"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PageInfo 属性。获取或设置 PageLegend 类的实例，该类指定页面图例的渲染选项"
type: docs
weight: 40
url: /zh/net/aspose.tasks.visualization/pageinfo/legend/
---
## PageInfo.Legend property

获取或设置 [`PageLegend`](../../pagelegend/) 类的实例，该类指定页面图例的渲染选项。

```csharp
public PageLegend Legend { get; set; }
```

## 备注

当前仅适用于甘特图视图。

## 示例

展示如何使用页面图例信息。

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// 让我们读取页面图例信息
var legend = project.DefaultView.PageInfo.Legend;

Console.WriteLine("Legend left text: {0} ", legend.LeftText);
Console.WriteLine("Legend left image: {0} ", legend.LeftImage);
Console.WriteLine("Legend center text: {0} ", legend.CenteredText);
Console.WriteLine("Legend center image: {0} ", legend.CenteredImage);
Console.WriteLine("Legend right text: {0} ", legend.RightText);
Console.WriteLine("Legend right image: {0} ", legend.RightImage);
Console.WriteLine("Legend On: {0} ", legend.LegendOn);
Console.WriteLine("Legend Width: {0} ", legend.Width);

// 还支持对图例的修改
legend.LeftText = "New Left Text";

project.Save(OutDir + "WorkWithPageLegend_out.mpp", SaveFileFormat.Mpp);
```

展示如何使用 MS Project 视图的页面信息。

```csharp
var project = new Project(DataDir + "Project2.mpp");

// 让我们修改默认视图
var info = project.DefaultView.PageInfo;

Console.WriteLine("Modify Page Info: " + info.Name);

// 让我们修改边距
info.Margins.Left = 10d;
info.Margins.Top = 10d;
info.Margins.Right = 10d;
info.Margins.Bottom = 10d;

// 让我们修改页面设置
info.PageSettings.IsPortrait = true;
info.PageSettings.PaperSize = PrinterPaperSize.PaperA4;

// 让我们修改页面视图设置
// 设置一个值，指示是否打印备注。
info.PageViewSettings.PrintNotes = true;

var header = new HeaderFooterInfo
{
    LeftText = "Left header text",
    CenteredText = "Centered header text",
    RightText = "Right header text"
};
var legend = new PageLegend
{
    LeftText =  "Left legend text",
    CenteredText = "Centered legend text",
    RightText = "Right legend text"
};
var footer = new HeaderFooterInfo
{
    LeftText = "Left footer text",
    CenteredText = "Centered footer text",
    RightText = "Right footer text"
};

info.Header = header;
info.Legend = legend;
info.Footer = footer;

// 处理项目...
```

### 另见

* class [PageLegend](../../pagelegend/)
* class [PageInfo](../)
* namespace [Aspose.Tasks.Visualization](../../pageinfo/)
* assembly [Aspose.Tasks](../../../)


