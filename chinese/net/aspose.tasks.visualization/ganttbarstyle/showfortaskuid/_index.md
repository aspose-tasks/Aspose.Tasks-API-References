---
title: "GanttBarStyle.ShowForTaskUid"
second_title: "Aspose.Tasks for .NET API 参考"
description: "GanttBarStyle 属性。获取或设置样式应用的任务的唯一标识。适用于甘特图中任务特定的栏样式，参见 CustomBarStyles"
type: docs
weight: 210
url: /zh/net/aspose.tasks.visualization/ganttbarstyle/showfortaskuid/
---
## GanttBarStyle.ShowForTaskUid property

获取或设置样式应用的任务的唯一标识。适用于甘特图中任务特定的栏样式（参见 [`CustomBarStyles`](../../../aspose.tasks/ganttchartview/custombarstyles/)）。

```csharp
public int? ShowForTaskUid { get; set; }
```

## 示例

展示如何使用 ShowFor 类别。

```csharp
var project = new Project(DataDir + "Project2.mpp");
var view = (GanttChartView)project.DefaultView;

var barStyle = this.GetCustomBarStyle();
barStyle.ShowForTaskUid = null;

var showForCategories = new[]
{
    GanttBarShowFor.Active,
    GanttBarShowFor.NotSummary,
    GanttBarShowFor.Milestone,
    GanttBarShowFor.Finished
};

barStyle.ShowForCategories = new List<GanttBarShowFor>(showForCategories);
barStyle.Name = "My common style";
view.BarStyles.Add(barStyle);

// 处理项目...
```

### 另见

* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


