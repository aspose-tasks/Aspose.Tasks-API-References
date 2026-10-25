---
title: "枚举 TimescaleUnit"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.TimescaleUnit 枚举。指定甘特图或其他时间分段视图中时间刻度任意层级的时间单位。"
type: docs
weight: 3460
url: /zh/net/aspose.tasks.visualization/timescaleunit/
---
## TimescaleUnit enumeration

指定甘特图或其他时间分段视图中时间尺度任意层级的时间单位。

```csharp
public enum TimescaleUnit
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| None | `-1` | 表示无。时间刻度层级被隐藏。 |
| Minutes | `0` | 表示分钟时间单位。 |
| Hours | `1` | 表示小时时间单位。 |
| Days | `2` | 表示天时间单位。 |
| Weeks | `3` | 表示周时间单位。 |
| ThirdsOfMonths | `4` | 表示月的三分之一时间单位。 |
| Months | `5` | 表示月时间单位。 |
| Quarters | `6` | 表示年的季度时间单位。 |
| HalfYears | `7` | 表示半年时间单位。 |
| Years | `8` | 表示年时间单位。 |

## 示例

展示如何自定义时间尺度层级标签。

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// 添加任务链接
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// 调优时间尺度层级

// 调优顶部层级
// 设置甘特图视图的顶部时间尺度层级。
view.MiddleTimescaleTier = new TimescaleTier();
// 为时间尺度层级设置时间尺度单位 <see cref="T:Aspose.Tasks.Visualization.TimescaleUnit" />。
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// 设置在层级中显示标签的时间单位间隔。
view.MiddleTimescaleTier.Count = 1;
// 为时间尺度层级设置日期标签 <see cref="T:Aspose.Tasks.Visualization.DateLabel" />。
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// 设置在层级的每个时间段内对齐标签的方式 (<see cref="T:System.Drawing.StringAlignment" />)。
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// 设置一个值，指示是否在层级中显示分隔时间段的刻度线。
view.MiddleTimescaleTier.ShowTicks = true;
// 设置一个值，指示是否基于财政年度来确定层级标签。
view.MiddleTimescaleTier.UsesFiscalYear = true;

// 为获得更好的可视化而添加。
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// 自定义中间层级的日期
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// 使用 'Timescale.DefinedInView' 选项，根据视图中定义的时间尺度设置（view.TopTimescaleTier、view.MiddleTimescaleTier、view.BottomTimescaleTier）渲染时间尺度。
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### 另见

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


