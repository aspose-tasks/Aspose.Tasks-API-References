---
title: "GanttBarStyle.Name"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété GanttBarStyle. Obtient ou définit le nom du style"
type: docs
weight: 150
url: /fr/net/aspose.tasks.visualization/ganttbarstyle/name/
---
## GanttBarStyle.Name property

Obtient ou définit le nom du style.

```csharp
public string Name { get; set; }
```

## Exemples

Montre comment utiliser les catégories ShowFor.

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

// travailler avec le projet...
```

### Voir aussi

* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


