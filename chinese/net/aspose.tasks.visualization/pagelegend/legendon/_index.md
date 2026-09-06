---
title: "PageLegend.LegendOn"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PageLegend 属性。获取或设置图例出现的页面。可以是 Legend 枚举的其中一个值。"
type: docs
weight: 20
url: /zh/net/aspose.tasks.visualization/pagelegend/legendon/
---
## PageLegend.LegendOn property

获取或设置图例出现的页面。可以是 [`Legend`](../../legend/) 枚举的其中一个值。

```csharp
public Legend LegendOn { get; set; }
```

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

* enum [Legend](../../legend/)
* class [PageLegend](../)
* namespace [Aspose.Tasks.Visualization](../../pagelegend/)
* assembly [Aspose.Tasks](../../../)


