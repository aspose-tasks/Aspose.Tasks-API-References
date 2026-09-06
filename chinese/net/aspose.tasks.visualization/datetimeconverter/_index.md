---
title: "委托 DateTimeConverter"
second_title: "Aspose.Tasks for .NET API 参考"
description: "表示一种转换方法，用于在视图时间尺度层中将日期转换为字符串"
type: docs
weight: 2990
url: /zh/net/aspose.tasks.visualization/datetimeconverter/
---
## DateTimeConverter delegate

表示用于在视图时间刻度层中将日期转换为字符串的转换方法。

```csharp
public delegate string DateTimeConverter(DateTime date);
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 日期 | DateTime | 要转换为字符串的 DateTime 类的实例。 |

### 返回值

指定日期的字符串表示形式。

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


