---
title: "GanttBarStyle.ShowForCategories"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété GanttBarStyle. Obtient ou définit les catégories de tâches pour lesquelles le style est appliqué. Applicable aux styles parent ou communs des barres dans le diagramme de Gantt, voir BarStyles"
type: docs
weight: 200
url: /fr/net/aspose.tasks.visualization/ganttbarstyle/showforcategories/
---
## GanttBarStyle.ShowForCategories property

Obtient ou définit les catégories de tâches pour lesquelles le style est appliqué. Applicable aux styles parent (ou communs) des barres dans le diagramme de Gantt (voir [`BarStyles`](../../../aspose.tasks/ganttchartview/barstyles/)).

```csharp
public IList<GanttBarShowFor> ShowForCategories { get; set; }
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

* enum [GanttBarShowFor](../../ganttbarshowfor/)
* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


