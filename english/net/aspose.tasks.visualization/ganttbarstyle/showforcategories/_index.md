---
title: GanttBarStyle.ShowForCategories
second_title: Aspose.Tasks for .NET API Reference
description: GanttBarStyle property. Gets or sets task categories for which the style is applied. Is applicable for parent or common styles of bars in Gantt chart see BarStyles
type: docs
weight: 200
url: /net/aspose.tasks.visualization/ganttbarstyle/showforcategories/
---
## GanttBarStyle.ShowForCategories property

Gets or sets task categories for which the style is applied. Is applicable for parent (or common) styles of bars in Gantt chart (see [`BarStyles`](../../../aspose.tasks/ganttchartview/barstyles/)).

```csharp
public IList<GanttBarShowFor> ShowForCategories { get; set; }
```

## Examples

Shows how to use ShowFor categories.

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

// work with project...
```

### See Also

* enum [GanttBarShowFor](../../ganttbarshowfor/)
* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


