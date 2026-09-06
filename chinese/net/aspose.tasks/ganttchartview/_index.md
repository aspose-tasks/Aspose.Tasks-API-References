---
title: "类 GanttChartView"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.GanttChartView 类。表示甘特图视图"
type: docs
weight: 710
url: /zh/net/aspose.tasks/ganttchartview/
---
## GanttChartView class

表示 GanttChart 视图。

```csharp
public class GanttChartView : View
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [GanttChartView](ganttchartview/)() | 初始化 `GanttChartView` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [AutoFilters](../../aspose.tasks/ganttchartview/autofilters/) { get; } | 获取甘特图视图的自动过滤器列表。 |
| [BarRounding](../../aspose.tasks/ganttchartview/barrounding/) { get; set; } | 获取或设置一个值，指示条形是否四舍五入到最近的天。默认值为 True。 |
| [BarSize](../../aspose.tasks/ganttchartview/barsize/) { get; set; } | 获取或设置甘特图中甘特条的高度（单位：点）。 |
| [BarStyles](../../aspose.tasks/ganttchartview/barstyles/) { get; } | 获取甘特图视图的父（通用）条样式列表。[`GanttBarStyle`](../../aspose.tasks.visualization/ganttbarstyle/)。 |
| [BottomTimescaleTier](../../aspose.tasks/ganttchartview/bottomtimescaletier/) { get; set; } | 获取或设置视图底部时间刻度层的设置。[`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/) |
| [CustomBarStyles](../../aspose.tasks/ganttchartview/custombarstyles/) { get; } | 获取甘特图视图的自定义任务特定条样式列表。[`GanttBarStyle`](../../aspose.tasks.visualization/ganttbarstyle/)。 |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | 获取或设置在单视图中使用的过滤器。 |
| [Gridlines](../../aspose.tasks/ganttchartview/gridlines/) { get; set; } | 获取或设置甘特图视图的 [`Gridlines`](./gridlines/) 列表。 |
| [Group](../../aspose.tasks/view/group/) { get; set; } | 获取或设置单视图的组。 |
| [HideRollupBarsWhenSummaryExpanded](../../aspose.tasks/ganttchartview/hiderollupbarswhensummaryexpanded/) { get; set; } | 获取或设置一个值，指示在展开汇总任务时是否隐藏汇总条。 |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | 获取或设置一个值，指示 Microsoft Project 是否突出显示单视图的过滤器。 |
| [MiddleTimescaleTier](../../aspose.tasks/ganttchartview/middletimescaletier/) { get; set; } | 获取或设置视图的中间时间刻度层设置。[`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/)。 |
| [Name](../../aspose.tasks/view/name/) { get; set; } | 获取或设置 View 对象的名称。 |
| [NonWorkingTimeColor](../../aspose.tasks/ganttchartview/nonworkingtimecolor/) { get; set; } | 获取或设置非工作时间的颜色。 |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | 获取 [`PageInfo`](../view/pageinfo/) 类的实例。表示存在于 mpp 文件格式中的页面设置数据。 |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | 获取 View 对象的父对象。只读 [`Project`](../project/)。 |
| [ProgressLines](../../aspose.tasks/ganttchartview/progresslines/) { get; set; } | 获取或设置甘特图视图的进度线。[`ProgressLines`](./progresslines/)。 |
| [RollUpGanttBars](../../aspose.tasks/ganttchartview/rollupganttbars/) { get; set; } | 获取或设置一个值，指示甘特图上的条是否必须进行汇总。 |
| [Screen](../../aspose.tasks/view/screen/) { get; } | 获取单视图的屏幕类型。只读 [`ViewScreen`](../viewscreen/)。 |
| [ShowBarSplits](../../aspose.tasks/ganttchartview/showbarsplits/) { get; set; } | 获取或设置一个值，指示甘特图上是否必须显示任务拆分。 |
| [ShowDrawings](../../aspose.tasks/ganttchartview/showdrawings/) { get; set; } | 获取或设置一个值，指示甘特图上是否必须显示绘图。 |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | 获取或设置一个值，指示 Microsoft Project 是否在功能区的视图或其他视图下拉列表中显示单视图名称。 |
| [Table](../../aspose.tasks/view/table/) { get; set; } | 获取或设置单视图的表格。 |
| [TableTextStyles](../../aspose.tasks/ganttchartview/tabletextstyles/) { get; } | 获取甘特图视图的表格文本样式列表。[`TableTextStyle`](../../aspose.tasks.visualization/tabletextstyle/)。 |
| [TextStyles](../../aspose.tasks/ganttchartview/textstyles/) { get; set; } | 获取或设置甘特图视图的 [`TextStyle`](../../aspose.tasks.visualization/textstyle/) 列表。 |
| [TimescaleSizePercentage](../../aspose.tasks/ganttchartview/timescalesizepercentage/) { get; set; } |  |
| [TopTimescaleTier](../../aspose.tasks/ganttchartview/toptimescaletier/) { get; set; } | 获取或设置视图的顶部时间刻度层设置。[`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/)。 |
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

### 另见

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


