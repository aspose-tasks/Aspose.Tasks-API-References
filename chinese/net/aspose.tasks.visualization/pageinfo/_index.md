---
title: "类 PageInfo"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.PageInfo 类。表示在 MPP 文件格式中存在并用于打印的页面设置数据。"
type: docs
weight: 3200
url: /zh/net/aspose.tasks.visualization/pageinfo/
---
## PageInfo class

表示存在于 MPP 文件格式中并用于打印的页面设置数据。

```csharp
public class PageInfo
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [PageInfo](pageinfo/)() | 初始化 `PageInfo` 类的新实例。表示在 MPP 文件格式中存在并用于打印的页面设置数据。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Footer](../../aspose.tasks.visualization/pageinfo/footer/) { get; set; } | 获取或设置 [`HeaderFooterInfo`](../headerfooterinfo/) 类的实例，该实例表示页脚数据。 |
| [Header](../../aspose.tasks.visualization/pageinfo/header/) { get; set; } | 获取或设置 [`HeaderFooterInfo`](../headerfooterinfo/) 类的实例，该实例表示页眉数据。 |
| [Legend](../../aspose.tasks.visualization/pageinfo/legend/) { get; set; } | 获取或设置 [`PageLegend`](../pagelegend/) 类的实例，该实例指定页面图例的渲染选项。 |
| [Margins](../../aspose.tasks.visualization/pageinfo/margins/) { get; } | 获取 [`PageMargins`](../pagemargins/) 类的实例，该实例指定页面边距。 |
| [Name](../../aspose.tasks.visualization/pageinfo/name/) { get; } | 获取使用设置数据的视图名称。 |
| [PageSettings](../../aspose.tasks.visualization/pageinfo/pagesettings/) { get; } | 获取 [`PageSettings`](./pagesettings/) 类的实例，该实例指定页面打印设置。 |
| [PageViewSettings](../../aspose.tasks.visualization/pageinfo/pageviewsettings/) { get; } | 获取 [`PageViewSettings`](./pageviewsettings/) 类的实例，该实例指定页面视图打印设置。 |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


