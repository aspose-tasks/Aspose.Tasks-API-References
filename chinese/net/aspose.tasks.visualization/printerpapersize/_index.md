---
title: "枚举 PrinterPaperSize"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.PrinterPaperSize 枚举。指定用于打印的纸张尺寸"
type: docs
weight: 3280
url: /zh/net/aspose.tasks.visualization/printerpapersize/
---
## PrinterPaperSize enumeration

指定用于打印的纸张尺寸。

```csharp
public enum PrinterPaperSize
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Custom | `1` | 指示纸张尺寸由用户定义。 |
| PaperLetter | `1` | 指示信封信件打印纸尺寸 (8.5 in. by 11 in.). |
| PaperLetterSmall | `2` | 指示小号信件打印纸尺寸 (8.5 in. by 11 in.). |
| PaperTabloid | `3` | 指示小报打印纸尺寸 (11 in. by 17 in.). |
| PaperLedger | `4` | 指示账本打印纸尺寸 (17 in. by 11 in.). |
| PaperLegal | `5` | 指示信封法律打印纸尺寸 (8.5 in. by 14 in.). |
| PaperStatement | `6` | 指示报表打印纸尺寸 (5.5 in. by 8.5 in.). |
| PaperExecutive | `7` | 指示信封行政打印纸尺寸 (7.25 in. by 10.5 in.). |
| PaperA3 | `8` | 指示 A3 打印纸尺寸 (297 mm by 420 mm). |
| PaperA4 | `9` | 指示 A4 打印纸尺寸 (210 mm by 297 mm). |
| PaperA4Small | `10` | 指示小号 A4 打印纸尺寸 (210 mm by 297 mm). |
| PaperA5 | `11` | 指示 A5 打印纸尺寸 (148 mm by 210 mm). |
| PaperB4 | `12` | 指示 B4 打印纸尺寸 (250 mm by 353 mm). |
| PaperB5 | `13` | 指示 B5 打印纸尺寸 (176 mm by 250 mm). |
| PaperFolio | `14` | 指示对开本打印纸尺寸 (8.5 in. by 13 in.). |
| PaperQuarto | `15` | 指示四开本打印纸尺寸 (215 mm by 275 mm). |
| PaperStandard10x14 | `16` | 指示标准打印纸尺寸 (10 in. by 14 in.). |
| PaperStandard11x17 | `17` | 指示标准打印纸尺寸 (11 in. by 17 in.). |
| PaperNote | `18` | 指示便笺打印纸尺寸 (8.5 in. by 11 in.). |
| PaperEnvelope10 | `20` | 指示 Envelope10 打印纸尺寸 (4.125 in. by 9.5 in.). |
| PaperCSheet | `24` | 指示 C 纸打印纸尺寸 (17 in. by 22 in.). |
| PaperDSheet | `25` | 指示 D 纸打印纸尺寸 (22 in. by 34 in.). |
| PaperESheet | `26` | 指示 E 纸打印纸尺寸 (34 in. by 44 in.). |
| PaperEnvelopeMonarch | `37` | 指示信封 Monarch 打印纸尺寸 (3.875 in. by 7.5 in.). |
| PaperStandard9x11 | `44` | 指示标准打印纸尺寸 (9 in. by 11 in.). |
| PaperStandard10x11 | `45` | 指示标准打印纸尺寸 (10 in. by 11 in.). |
| PaperStandard15x11 | `46` | 指示标准打印纸尺寸（15 英寸 x 11 英寸）。 |
| PaperA2 | `66` | 指示 A2 打印纸尺寸（420 毫米 x 594 毫米）。 |

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


