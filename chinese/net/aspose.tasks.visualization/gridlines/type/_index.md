---
title: "Gridlines.Type"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Gridlines 属性。获取或设置网格线类型"
type: docs
weight: 70
url: /zh/net/aspose.tasks.visualization/gridlines/type/
---
## Gridlines.Type property

获取或设置网格线类型。

```csharp
public GridlineType Type { get; set; }
```

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

* enum [GridlineType](../../gridlinetype/)
* class [Gridlines](../)
* namespace [Aspose.Tasks.Visualization](../../gridlines/)
* assembly [Aspose.Tasks](../../../)


