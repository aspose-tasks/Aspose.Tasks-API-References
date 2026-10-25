---
title: "TimelineView.TextLinesCount"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TimelineView 属性。获取或设置一个值，指示在时间轴中显示任务时使用的行数"
type: docs
weight: 80
url: /zh/net/aspose.tasks/timelineview/textlinescount/
---
## TimelineView.TextLinesCount property

获取或设置一个值，指示在时间轴中用于显示任务的行数。

```csharp
public int TextLinesCount { get; set; }
```

## 示例

展示如何使用 &lt;see cref="Aspose.Tasks.TimelineView" /&gt;。

```csharp
var project = new Project();

// 初始化时间轴视图
var view = new TimelineView();

// 设置一个值，指示在时间轴视图上如何格式化日期。
view.DateFormat = DateFormat.DateDddDd;
// 设置一个值，指示是否在多行上显示重叠的任务。
view.DisplayOverlapped = true;
// 设置一个值，指示是否显示平移和缩放控件。
view.ShowPanZoom = true;
// 设置一个值，指示是否显示时间刻度。
view.ShowTimescale = true;
// 设置一个值，指示是否显示表示今天的线。
view.ShowToday = true;
// 设置一个值，指示在时间轴中用于显示任务的行数。
view.TextLinesCount = 2;

// 获取一个值，指示是否在多行上显示重叠的任务。
Console.WriteLine("Show Dates: " + view.ShowDates);

// 将视图添加到项目中
project.Views.Add(view);

// 向项目添加一些测试数据
var task1 = project.RootTask.Children.Add("Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

project.Save(OutDir + "SetTimeScaleCount_out.pdf", SaveFileFormat.Pdf);
```

### 另见

* class [TimelineView](../)
* namespace [Aspose.Tasks](../../timelineview/)
* assembly [Aspose.Tasks](../../../)


