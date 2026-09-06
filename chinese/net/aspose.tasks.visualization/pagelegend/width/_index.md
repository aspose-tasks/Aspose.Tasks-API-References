---
title: "PageLegend.Width"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PageLegend 属性。获取或设置图例左侧部分（默认包含项目名称和日期）的宽度，单位为厘米"
type: docs
weight: 30
url: /zh/net/aspose.tasks.visualization/pagelegend/width/
---
## PageLegend.Width property

获取或设置图例左侧部分（默认包含项目名称和日期）的宽度（单位：厘米）。

```csharp
public double Width { get; set; }
```

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentOutOfRangeException | 当尝试设置为小于 0 的值时。 |

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

* class [PageLegend](../)
* namespace [Aspose.Tasks.Visualization](../../pagelegend/)
* assembly [Aspose.Tasks](../../../)


