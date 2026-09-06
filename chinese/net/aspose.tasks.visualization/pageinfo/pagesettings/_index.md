---
title: "PageInfo.PageSettings"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PageInfo 属性。获取 PageSettings 类的实例，该类指定页面打印设置"
type: docs
weight: 70
url: /zh/net/aspose.tasks.visualization/pageinfo/pagesettings/
---
## PageInfo.PageSettings property

获取 `PageSettings` 类的实例，该类指定页面打印设置。

```csharp
public PageSettings PageSettings { get; }
```

## 示例

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

* class [PageSettings](../../pagesettings/)
* class [PageInfo](../)
* namespace [Aspose.Tasks.Visualization](../../pageinfo/)
* assembly [Aspose.Tasks](../../../)


