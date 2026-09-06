---
title: "Project.DefaultView"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 属性。获取或设置项目的默认视图"
type: docs
weight: 360
url: /zh/net/aspose.tasks/project/defaultview/
---
## Project.DefaultView property

获取或设置项目的默认视图。

```csharp
public View DefaultView { get; set; }
```

## 示例

展示如何使用项目的默认视图。

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// 获取默认视图
UsageView view = (TaskUsageView)project.DefaultView;

// 详情标题列将不显示
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// 显示详情标题列
view.DisplayDetailsHeaderColumn = true;

// 在所有分配行上重复显示详情标题
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

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

### 另见

* class [View](../../view/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


