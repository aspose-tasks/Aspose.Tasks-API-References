---
title: "GanttBarStyle.ShowForTaskUid"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "GanttBarStyle eigenschap. Haalt op of stelt een unieke ID van een taak in waarvoor de stijl wordt toegepast. Van toepassing op taakspecifieke stijlen van balken in een Gantt-diagram, zie CustomBarStyles"
type: docs
weight: 210
url: /nl/net/aspose.tasks.visualization/ganttbarstyle/showfortaskuid/
---
## GanttBarStyle.ShowForTaskUid property

Haalt op of stelt een unieke ID van een taak in waarvoor de stijl wordt toegepast. Van toepassing op taakspecifieke stijlen van balken in een Gantt-diagram (zie [`CustomBarStyles`](../../../aspose.tasks/ganttchartview/custombarstyles/)).

```csharp
public int? ShowForTaskUid { get; set; }
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


