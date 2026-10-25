---
title: "GanttBarStyle.Name"
second_title: "Aspose.Tasks for .NET API 参考"
description: "GanttBarStyle 属性。获取或设置样式的名称"
type: docs
weight: 150
url: /zh/net/aspose.tasks.visualization/ganttbarstyle/name/
---
## GanttBarStyle.Name property

获取或设置样式的名称。

```csharp
public string Name { get; set; }
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


