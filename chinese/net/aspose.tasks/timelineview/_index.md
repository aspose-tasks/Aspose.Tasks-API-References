---
title: "类 TimelineView"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.TimelineView 类。表示项目的时间轴视图"
type: docs
weight: 2580
url: /zh/net/aspose.tasks/timelineview/
---
## TimelineView class

表示项目的时间线视图。

```csharp
public class TimelineView : View
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [TimelineView](timelineview/)() | 初始化 `TimelineView` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [DateFormat](../../aspose.tasks/timelineview/dateformat/) { get; set; } | 获取或设置一个值，指示在时间轴视图上如何格式化日期。 |
| [DisplayOverlapped](../../aspose.tasks/timelineview/displayoverlapped/) { get; set; } | 获取或设置一个值，指示是否在多行上显示重叠的任务。 |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | 获取或设置在单视图中使用的过滤器。 |
| [Group](../../aspose.tasks/view/group/) { get; set; } | 获取或设置单视图的组。 |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | 获取或设置一个值，指示 Microsoft Project 是否突出显示单视图的过滤器。 |
| [Name](../../aspose.tasks/view/name/) { get; set; } | 获取或设置 View 对象的名称。 |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | 获取 [`PageInfo`](../view/pageinfo/) 类的实例。表示存在于 mpp 文件格式中的页面设置数据。 |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | 获取 View 对象的父对象。只读 [`Project`](../project/)。 |
| [Screen](../../aspose.tasks/view/screen/) { get; } | 获取单视图的屏幕类型。只读 [`ViewScreen`](../viewscreen/)。 |
| [ShowDates](../../aspose.tasks/timelineview/showdates/) { get; } | 获取一个值，指示是否显示日期。 |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | 获取或设置一个值，指示 Microsoft Project 是否在功能区的视图或其他视图下拉列表中显示单视图名称。 |
| [ShowPanZoom](../../aspose.tasks/timelineview/showpanzoom/) { get; set; } | 获取或设置一个值，指示是否显示平移和缩放控件。 |
| [ShowTimescale](../../aspose.tasks/timelineview/showtimescale/) { get; set; } | 获取或设置一个值，指示是否显示时间刻度。 |
| [ShowToday](../../aspose.tasks/timelineview/showtoday/) { get; set; } | 获取或设置一个值，指示是否显示表示今天的线。 |
| [Table](../../aspose.tasks/view/table/) { get; set; } | 获取或设置单视图的表格。 |
| [TextLinesCount](../../aspose.tasks/timelineview/textlinescount/) { get; set; } | 获取或设置一个值，指示在时间轴中用于显示任务的行数。 |
| [Type](../../aspose.tasks/view/type/) { get; } | 获取单视图中项目的类型，例如任务或资源。只读 [`ItemType`](../itemtype/)。 |
| [Uid](../../aspose.tasks/view/uid/) { get; } | 获取视图的唯一标识符。 |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | 获取表示视图中 [`OleObject`](../oleobject/) 的放置和外观的对象集合。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | 比较当前实例与同类型的另一个对象，并返回一个整数，指示当前实例在排序顺序中是位于前、后还是与另一个对象相同位置。 |
| override [Equals](../../aspose.tasks/view/equals/)(object) | 返回一个值，指示此实例是否等于指定的对象。 |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | 返回 [`Resource`](../resource/) 类实例的哈希码值。 |

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

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


