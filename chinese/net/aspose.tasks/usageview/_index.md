---
title: "类 UsageView"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.UsageView 类。表示项目中的使用视图。"
type: docs
weight: 2650
url: /zh/net/aspose.tasks/usageview/
---
## UsageView class

表示项目中的使用视图。

```csharp
public abstract class UsageView : View
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [AlignDetailsData](../../aspose.tasks/usageview/aligndetailsdata/) { get; set; } | 获取或设置详细数据对齐方式。 |
| [BottomTimescaleTier](../../aspose.tasks/usageview/bottomtimescaletier/) { get; set; } | 获取或设置视图底部时间刻度层的设置。[`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/) |
| [DisplayDetailsHeaderColumn](../../aspose.tasks/usageview/displaydetailsheadercolumn/) { get; set; } | 获取或设置一个值，指示是否在视图中显示详细标题列。 |
| [DisplayShortDetailHeaderNames](../../aspose.tasks/usageview/displayshortdetailheadernames/) { get; set; } | 获取或设置一个值，指示是否显示简短的详细标题名称。 |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | 获取或设置在单视图中使用的过滤器。 |
| [Group](../../aspose.tasks/view/group/) { get; set; } | 获取或设置单视图的组。 |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | 获取或设置一个值，指示 Microsoft Project 是否突出显示单视图的过滤器。 |
| [MiddleTimescaleTier](../../aspose.tasks/usageview/middletimescaletier/) { get; set; } | 获取或设置视图的中间时间刻度层设置。[`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/)。 |
| [Name](../../aspose.tasks/view/name/) { get; set; } | 获取或设置 View 对象的名称。 |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | 获取 [`PageInfo`](../view/pageinfo/) 类的实例。表示存在于 mpp 文件格式中的页面设置数据。 |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | 获取 View 对象的父对象。只读 [`Project`](../project/)。 |
| [RepeatDetailsHeaderOnAllRows](../../aspose.tasks/usageview/repeatdetailsheaderonallrows/) { get; set; } | 获取或设置一个值，指示是否在所有分配行上重复详细标题。 |
| [Screen](../../aspose.tasks/view/screen/) { get; } | 获取单视图的屏幕类型。只读 [`ViewScreen`](../viewscreen/)。 |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | 获取或设置一个值，指示 Microsoft Project 是否在功能区的视图或其他视图下拉列表中显示单视图名称。 |
| [Table](../../aspose.tasks/view/table/) { get; set; } | 获取或设置单视图的表格。 |
| [TimescaleSizePercentage](../../aspose.tasks/usageview/timescalesizepercentage/) { get; set; } |  |
| [TopTimescaleTier](../../aspose.tasks/usageview/toptimescaletier/) { get; set; } | 获取或设置视图的顶部时间刻度层设置。[`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/)。 |
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

展示如何渲染带有详细信息的任务使用视图。

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// 获取视图
UsageView view = (TaskUsageView)project.DefaultView;

// 详细标题列将不会显示
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.DisplayShortDetailHeaderNames = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// 显示详细标题列
view.DisplayDetailsHeaderColumn = true;

// 在所有分配行上重复详细标题
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

### 另见

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


