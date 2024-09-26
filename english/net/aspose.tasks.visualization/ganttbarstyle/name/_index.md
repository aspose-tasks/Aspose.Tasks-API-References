---
title: GanttBarStyle.Name
second_title: Aspose.Tasks for .NET API Reference
description: GanttBarStyle property. Gets or sets a name of the style
type: docs
weight: 150
url: /net/aspose.tasks.visualization/ganttbarstyle/name/
---
## GanttBarStyle.Name property

Gets or sets a name of the style.

```csharp
public string Name { get; set; }
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


