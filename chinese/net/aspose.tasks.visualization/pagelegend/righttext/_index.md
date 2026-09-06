---
title: "PageLegend.RightText"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PageLegend 属性。获取或设置在页面图例中显示的右对齐文本"
type: docs
weight: 80
url: /zh/net/aspose.tasks.visualization/pagelegend/righttext/
---
## PageLegend.RightText property

获取或设置在页面图例中显示的右对齐文本。

```csharp
public string RightText { get; set; }
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

* class [PageLegend](../)
* namespace [Aspose.Tasks.Visualization](../../pagelegend/)
* assembly [Aspose.Tasks](../../../)


