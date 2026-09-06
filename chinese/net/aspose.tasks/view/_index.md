---
title: "类 View"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.View 类。表示 Project 中的视图"
type: docs
weight: 2890
url: /zh/net/aspose.tasks/view/
---
## View class

表示 Project 中的视图。

```csharp
public class View : IComparable<View>
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [View](view/#constructor)() | 初始化 `View` 类的新实例。 |
| [View](view/#constructor_1)(ViewScreen) | 初始化 `View` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | 获取或设置在单视图中使用的过滤器。 |
| [Group](../../aspose.tasks/view/group/) { get; set; } | 获取或设置单视图的组。 |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | 获取或设置一个值，指示 Microsoft Project 是否突出显示单视图的过滤器。 |
| [Name](../../aspose.tasks/view/name/) { get; set; } | 获取或设置 View 对象的名称。 |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | 获取 [`PageInfo`](./pageinfo/) 类的实例。表示存在于 mpp 文件格式中的页面设置数据。 |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | 获取 View 对象的父对象。只读 [`Project`](../project/)。 |
| [Screen](../../aspose.tasks/view/screen/) { get; } | 获取单视图的屏幕类型。只读 [`ViewScreen`](../viewscreen/)。 |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | 获取或设置一个值，指示 Microsoft Project 是否在功能区的视图或其他视图下拉列表中显示单视图名称。 |
| [Table](../../aspose.tasks/view/table/) { get; set; } | 获取或设置单视图的表格。 |
| [Type](../../aspose.tasks/view/type/) { get; } | 获取单视图中项目的类型，例如任务或资源。只读 [`ItemType`](../itemtype/)。 |
| [Uid](../../aspose.tasks/view/uid/) { get; } | 获取视图的唯一标识符。 |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | 获取表示视图中 [`OleObject`](../oleobject/) 的放置和外观的对象集合。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | 比较当前实例与同类型的另一个对象，并返回一个整数，指示当前实例在排序顺序中是位于前、后还是与另一个对象相同位置。 |
| override [Equals](../../aspose.tasks/view/equals/)(object) | 返回一个值，指示此实例是否等于指定的对象。 |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | 返回 [`Resource`](../resource/) 类实例的哈希码值。 |
| [operator ==](../../aspose.tasks/view/op_equality/) | 返回一个值，指示此实例是否等于指定的对象。 |
| [operator &gt;](../../aspose.tasks/view/op_greaterthan/) | 返回一个值，指示此实例是否大于指定的对象。 |
| [operator &gt;=](../../aspose.tasks/view/op_greaterthanorequal/) | 返回一个值，指示此实例是否大于或等于指定的对象。 |
| [operator !=](../../aspose.tasks/view/op_inequality/) | 返回一个值，指示此实例是否不等于指定的对象。 |
| [operator &lt;](../../aspose.tasks/view/op_lessthan/) | 返回一个值，指示此实例是否小于指定的对象。 |
| [operator &lt;=](../../aspose.tasks/view/op_lessthanorequal/) | 返回一个值，指示此实例是否小于或等于指定的对象。 |

## 示例

展示如何使用 Project 的视图并向默认视图添加列（当在 MS Project 中打开 MPP 文件时显示的视图）。

```csharp
// 创建一个没有视图的空项目
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// 修改默认视图（它是甘特图视图）。
// 或者您可以使用 project.View 集合通过名称或通过视图屏幕选择视图。
var view = (GanttChartView) project.DefaultView;

TableField newColumn = new TableField()
{
    AlignData = HorizontalStringAlignment.Center,
    Title = "My new column",
    Width = 30,
    Field = Field.TaskActualDuration
};

view.Table.TableFields.Add(newColumn);

// 应使用 WriteViewData 标志来持久化视图属性的修改。
project.Save(OutDir + "ModifyView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
```

展示如何使用 MS Project 视图。

```csharp
// 创建一个没有视图的空项目
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// 创建标准甘特图视图
View view = new GanttChartView();

// 设置一些视图属性
// 设置一个值，指示 Microsoft Project 是否在功能区的 View 或 Other Views 下拉列表中显示单个视图名称
view.ShowInMenu = true;
// 设置一个值，指示 Microsoft Project 是否突出显示单个视图的过滤器
view.HighlightFilter = true;

// 不支持写入以下属性
// 设置单个视图使用的过滤器
view.Filter = null;
// 设置单个视图的分组
view.Group = null;
// 设置单个视图的表格
view.Table = null;

// 让我们调整一些视图设置
// 设置所有页面上要打印的首列数量
view.PageInfo.PageViewSettings.FirstColumnsCount = 4;
// 设置一个值，指示是否在所有页面上打印指定数量的首列
view.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

// 将视图添加到我们的项目中
project.Views.Add(view);

// 应使用 WriteViewData 标志来持久化 project.Views 的修改。
project.Save(OutDir + "WorkWithView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
// 让我们检查新添加视图的一些属性
// 打印视图的唯一标识符
Console.WriteLine("View Uid: " + view.Uid);
// 打印单个视图的屏幕类型
Console.WriteLine("View Screen: " + view.Screen);
Console.WriteLine("View Type: " + view.Type);
Console.WriteLine("Parent Project of the view: " + view.ParentProject.Get(Prj.Name));
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


