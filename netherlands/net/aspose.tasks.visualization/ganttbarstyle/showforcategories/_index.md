---
title: "GanttBarStyle.ShowForCategories"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "GanttBarStyle-eigenschap. Haalt op of stelt taakcategorieën in waarvoor de stijl wordt toegepast. Is van toepassing op bovenliggende of gemeenschappelijke stijlen van balken in een Gantt‑diagram, zie BarStyles."
type: docs
weight: 200
url: /nl/net/aspose.tasks.visualization/ganttbarstyle/showforcategories/
---
## GanttBarStyle.ShowForCategories property

Haalt op of stelt taakcategorieën in waarvoor de stijl wordt toegepast. Is van toepassing op bovenliggende (of gemeenschappelijke) stijlen van balken in een Gantt‑diagram (zie [`BarStyles`](../../../aspose.tasks/ganttchartview/barstyles/)).

```csharp
public IList<GanttBarShowFor> ShowForCategories { get; set; }
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

* enum [GanttBarShowFor](../../ganttbarshowfor/)
* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


