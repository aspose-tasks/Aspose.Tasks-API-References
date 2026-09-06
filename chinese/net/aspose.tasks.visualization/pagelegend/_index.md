---
title: "类 PageLegend"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.PageLegend 类。表示用于项目打印的页面图例。"
type: docs
weight: 3210
url: /zh/net/aspose.tasks.visualization/pagelegend/
---
## PageLegend class

表示用于项目打印的页面图例。

```csharp
public class PageLegend : HeaderFooterInfo
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [PageLegend](pagelegend/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [CenteredImage](../../aspose.tasks.visualization/headerfooterinfo/centeredimage/) { get; set; } | 获取或设置在父元素中显示的居中图像。 |
| [CenteredImageSize](../../aspose.tasks.visualization/headerfooterinfo/centeredimagesize/) { get; set; } | 获取或设置居中图像的显示尺寸。 |
| [CenteredText](../../aspose.tasks.visualization/headerfooterinfo/centeredtext/) { get; set; } | 获取或设置在父元素中显示的居中文本。 |
| [LeftImage](../../aspose.tasks.visualization/headerfooterinfo/leftimage/) { get; set; } | 获取或设置在父元素中显示的左对齐图像。 |
| [LeftImageSize](../../aspose.tasks.visualization/headerfooterinfo/leftimagesize/) { get; set; } | 获取或设置左图像的显示尺寸。 |
| [LeftText](../../aspose.tasks.visualization/headerfooterinfo/lefttext/) { get; set; } | 获取或设置在父元素中显示的左对齐文本。 |
| [LegendOn](../../aspose.tasks.visualization/pagelegend/legendon/) { get; set; } | 获取或设置图例出现的页面。可以是 [`Legend`](../legend/) 枚举的其中一个值。 |
| [RightImage](../../aspose.tasks.visualization/headerfooterinfo/rightimage/) { get; set; } | 获取或设置在父元素中显示的右对齐图像。 |
| [RightImageSize](../../aspose.tasks.visualization/headerfooterinfo/rightimagesize/) { get; set; } | 获取或设置右图像的显示尺寸。 |
| [RightText](../../aspose.tasks.visualization/headerfooterinfo/righttext/) { get; set; } | 获取或设置在父元素中显示的右对齐文本。 |
| [Width](../../aspose.tasks.visualization/pagelegend/width/) { get; set; } | 获取或设置图例左侧部分（默认包含项目名称和日期）的宽度（单位：厘米）。 |

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

### 另见

* class [HeaderFooterInfo](../headerfooterinfo/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


