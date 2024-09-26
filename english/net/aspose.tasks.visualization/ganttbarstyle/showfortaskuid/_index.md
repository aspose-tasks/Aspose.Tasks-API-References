---
title: GanttBarStyle.ShowForTaskUid
second_title: Aspose.Tasks for .NET API Reference
description: GanttBarStyle property. Gets or sets Unique Id of a task for which the style is applied. Is applicable for taskspecific styles of bars in Gantt chart see CustomBarStyles
type: docs
weight: 210
url: /net/aspose.tasks.visualization/ganttbarstyle/showfortaskuid/
---
## GanttBarStyle.ShowForTaskUid property

Gets or sets Unique Id of a task for which the style is applied. Is applicable for task-specific styles of bars in Gantt chart (see [`CustomBarStyles`](../../../aspose.tasks/ganttchartview/custombarstyles/)).

```csharp
public int? ShowForTaskUid { get; set; }
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

* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


