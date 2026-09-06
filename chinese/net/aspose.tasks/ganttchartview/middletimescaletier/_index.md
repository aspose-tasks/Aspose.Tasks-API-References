---
title: "GanttChartView.MiddleTimescaleTier"
second_title: "Aspose.Tasks for .NET API 参考"
description: "GanttChartView 属性。获取或设置视图中间时间刻度层的设置。TimescaleTier"
type: docs
weight: 100
url: /zh/net/aspose.tasks/ganttchartview/middletimescaletier/
---
## GanttChartView.MiddleTimescaleTier property

获取或设置视图的中间时间尺度层的设置。[`TimescaleTier`](../../../aspose.tasks.visualization/timescaletier/)。

```csharp
public TimescaleTier MiddleTimescaleTier { get; set; }
```

## 示例

展示如何通过保存选项使用时间刻度层。

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

GanttChartView ganttChartView = (GanttChartView) project.Views.ToList()[0];

// 设置 Gantt Chart 视图的时间刻度层
ganttChartView.MiddleTimescaleTier.Unit = TimescaleUnit.Months;
ganttChartView.MiddleTimescaleTier.Count = 1;
ganttChartView.MiddleTimescaleTier.Label = DateLabel.MonthMmmm;

ganttChartView.BottomTimescaleTier.Unit = TimescaleUnit.Days;
ganttChartView.BottomTimescaleTier.Count = 1;
ganttChartView.BottomTimescaleTier.Label = DateLabel.DayDddDd;

// ...
var options = new ImageSaveOptions(SaveFileFormat.Png)
{
    Timescale = Timescale.DefinedInView
};

// ...

// 将项目保存为图像
project.Save(OutDir + "WorkWithTimescaleTier_out.png", options);
```

展示如何修改时间尺度层级。

```csharp
var project = new Project();

// 初始化甘特图视图
var view = new GanttChartView
{
    TopTimescaleTier = new TimescaleTier(),
    MiddleTimescaleTier = new TimescaleTier(),
    BottomTimescaleTier = new TimescaleTier()
};

// 设置时间尺度计数
view.TopTimescaleTier.Count = 2;
view.TopTimescaleTier.Unit = TimescaleUnit.Quarters;
view.TopTimescaleTier.Label = DateLabel.QuarterQQyy;
view.TopTimescaleTier.ShowTicks = false;

view.MiddleTimescaleTier.Count = 2;
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
view.MiddleTimescaleTier.ShowTicks = false;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayDdd;
view.BottomTimescaleTier.Count = 2;
view.BottomTimescaleTier.ShowTicks = false;

// 将甘特图视图添加到项目中
project.Views.Add(view);

// 向项目添加一些测试数据
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

// 使用 'Timescale.DefinedInView' 选项，根据我们已设置的时间尺度设置（view.TopTimescaleTier、view.MiddleTimescaleTier、view.BottomTimescaleTier）渲染时间尺度。
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    StartDate = DateTime.Now.AddDays(-30),
    EndDate = DateTime.Now.AddDays(30)
};

project.Save(OutDir + "WorkWithTimescaleTier_out.pdf", pdfSaveOptions);
```

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

* class [TimescaleTier](../../../aspose.tasks.visualization/timescaletier/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


