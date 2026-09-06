---
title: "类 TimescaleTier"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.TimescaleTier 类。表示甘特图上时间尺度的单个层级"
type: docs
weight: 3450
url: /zh/net/aspose.tasks.visualization/timescaletier/
---
## TimescaleTier class

表示甘特图时间刻度的单个层级。

```csharp
public sealed class TimescaleTier
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [TimescaleTier](timescaletier/#constructor)() | 初始化 `TimescaleTier` 类的新实例。 |
| [TimescaleTier](timescaletier/#constructor_1)(TimescaleUnit, int) | 初始化 `TimescaleTier` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Alignment](../../aspose.tasks.visualization/timescaletier/alignment/) { get; set; } | 获取或设置在层级的每个时间段内对齐标签的方式（[`HorizontalStringAlignment`](../horizontalstringalignment/)）。 |
| [Count](../../aspose.tasks.visualization/timescaletier/count/) { get; set; } | 获取或设置在层级中显示标签的时间单位间隔。默认值为 1。 |
| [DateTimeConverter](../../aspose.tasks.visualization/timescaletier/datetimeconverter/) { get; set; } | 获取或设置用于处理此层级中日期刻度渲染的回调函数。 |
| [Label](../../aspose.tasks.visualization/timescaletier/label/) { get; set; } | 获取或设置时间尺度层级的日期标签 [`DateLabel`](../datelabel/)。 |
| [RenderLabelOnEachPage](../../aspose.tasks.visualization/timescaletier/renderlabeloneachpage/) { get; set; } | 获取或设置一个标志，定义当时间段跨越多个页面时是否在每页上渲染日期标签。如果值为 'true'，当时间段跨越多个页面时，期间的日期标签将在每页上渲染。如果值为 'false'，日期标签仅根据 [`Alignment`](./alignment/) 属性的值渲染一次。 |
| [ShowTicks](../../aspose.tasks.visualization/timescaletier/showticks/) { get; set; } | 获取或设置一个值，指示是否在层级中显示分隔时间段的刻度线。 |
| [Unit](../../aspose.tasks.visualization/timescaletier/unit/) { get; set; } | 获取或设置时间尺度层级的时间尺度单位 [`TimescaleUnit`](../timescaleunit/)。默认值为 [`Days`](../timescaleunit/)。 |
| [UsesFiscalYear](../../aspose.tasks.visualization/timescaletier/usesfiscalyear/) { get; set; } | 获取或设置一个值，指示是否基于财政年度来确定层级标签。 |

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


