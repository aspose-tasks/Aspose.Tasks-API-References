---
title: "类 Gridlines"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.Gridlines 类。表示出现在 GanttChart 视图中的网格线"
type: docs
weight: 3120
url: /zh/net/aspose.tasks.visualization/gridlines/
---
## Gridlines class

表示出现在甘特图视图中的网格线。

```csharp
public class Gridlines
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [Gridlines](gridlines/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Interval](../../aspose.tasks.visualization/gridlines/interval/) { get; set; } | 获取或设置 0 到 99 之间的数字，以指定网格线之间的间隔。 |
| [IntervalColor](../../aspose.tasks.visualization/gridlines/intervalcolor/) { get; set; } | 获取或设置次要网格线的颜色。 |
| [IntervalPattern](../../aspose.tasks.visualization/gridlines/intervalpattern/) { get; set; } | 获取或设置次要网格线的线型。 |
| [NormalColor](../../aspose.tasks.visualization/gridlines/normalcolor/) { get; set; } | 获取或设置普通网格线的颜色。 |
| [NormalPattern](../../aspose.tasks.visualization/gridlines/normalpattern/) { get; set; } | 获取或设置普通网格线的线型。 |
| [Type](../../aspose.tasks.visualization/gridlines/type/) { get; set; } | 获取或设置网格线类型。 |

## 示例

展示如何使用网格线。

```csharp
var project = new Project(DataDir + "Project2.mpp");

var view = (GanttChartView)project.Views.ToList()[0];

// 让我们调节视图的第一条网格线
var gridlines = view.Gridlines[0];
// 设置 0 到 99 之间的数字，以指定网格线之间的间隔。
gridlines.Interval = 2;
// 设置次要网格线的颜色。
gridlines.IntervalColor = Color.Red;
// 设置次要网格线的线型
gridlines.IntervalPattern = LinePattern.Solid;
// 设置普通网格线的颜色
gridlines.NormalColor = Color.Blue;
// 设置普通网格线的线型
gridlines.NormalPattern = LinePattern.CloseDot;
// 设置网格线类型
gridlines.Type = GridlineType.GanttRow;

project.Save(OutDir + "WorkWithGridlines_out.mpp", SaveFileFormat.Mpp);
```

### 另见

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


