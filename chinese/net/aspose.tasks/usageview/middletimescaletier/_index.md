---
title: "UsageView.MiddleTimescaleTier"
second_title: "Aspose.Tasks for .NET API 参考"
description: "UsageView 属性。获取或设置视图的中间时间尺度层的设置。TimescaleTier"
type: docs
weight: 50
url: /zh/net/aspose.tasks/usageview/middletimescaletier/
---
## UsageView.MiddleTimescaleTier property

获取或设置视图的中间时间尺度层的设置。[`TimescaleTier`](../../../aspose.tasks.visualization/timescaletier/)。

```csharp
public TimescaleTier MiddleTimescaleTier { get; set; }
```

## 示例

展示如何使用视图设置中定义的时间尺度设置渲染任务使用视图。

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.ToList()[2] as TaskUsageView;

view.TopTimescaleTier.Unit = TimescaleUnit.None;

view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddMDd;
view.MiddleTimescaleTier.Count = 1;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayMmDd;
view.BottomTimescaleTier.Count = 1;

// 定义 SaveOptions 并指定应使用 TaskUsageView 时间尺度设置。
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    PresentationFormat = PresentationFormat.TaskUsage
};

project.Save(OutDir + "TaskUsageView_CustomTimescale_out.pdf", options);
```

### 另见

* class [TimescaleTier](../../../aspose.tasks.visualization/timescaletier/)
* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


