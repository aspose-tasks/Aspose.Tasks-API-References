---
title: "View.ShowInMenu"
second_title: "Aspose.Tasks for .NET API 参考"
description: "View 属性。获取或设置一个值，指示 Microsoft Project 是否在功能区的“视图”或“其他视图”下拉列表中显示单个视图名称"
type: docs
weight: 90
url: /zh/net/aspose.tasks/view/showinmenu/
---
## View.ShowInMenu property

获取或设置一个值，指示 Microsoft Project 是否在功能区的视图或其他视图下拉列表中显示单视图名称。

```csharp
public bool ShowInMenu { get; set; }
```

## 示例

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

* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


