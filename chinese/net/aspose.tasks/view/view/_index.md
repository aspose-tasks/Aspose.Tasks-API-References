---
title: "View.View"
second_title: "Aspose.Tasks for .NET API 参考"
description: "View 构造函数。初始化 View 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks/view/view/
---
## View() {#constructor}

初始化 [`View`](../) 类的新实例。

```csharp
public View()
```

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

* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)

---

## View(ViewScreen) {#constructor_1}

初始化 [`View`](../) 类的新实例。

```csharp
public View(ViewScreen viewScreen)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| viewScreen | ViewScreen | 用于显示该视图的屏幕类型。 |

### 另见

* enum [ViewScreen](../../viewscreen/)
* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


