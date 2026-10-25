---
title: "GanttBarStyle.Name"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "GanttBarStyle eigenschap. Haalt op of stelt een naam van de stijl in"
type: docs
weight: 150
url: /nl/net/aspose.tasks.visualization/ganttbarstyle/name/
---
## GanttBarStyle.Name property

Geeft of stelt een naam van de stijl in.

```csharp
public string Name { get; set; }
```

## Voorbeelden

Toont hoe ShowFor-categorieën te gebruiken.

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

// werken met project...
```

### Zie ook

* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


