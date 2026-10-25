---
title: "GanttBarStyle.ShowForTaskUid"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété GanttBarStyle. Obtient ou définit l'Identifiant unique d'une tâche pour laquelle le style est appliqué. S'applique aux styles spécifiques aux tâches des barres dans le diagramme de Gantt, voir CustomBarStyles"
type: docs
weight: 210
url: /fr/net/aspose.tasks.visualization/ganttbarstyle/showfortaskuid/
---
## GanttBarStyle.ShowForTaskUid property

Obtient ou définit l'Identifiant unique d'une tâche pour laquelle le style est appliqué. S'applique aux styles spécifiques aux tâches des barres dans le diagramme de Gantt (voir [`CustomBarStyles`](../../../aspose.tasks/ganttchartview/custombarstyles/)).

```csharp
public int? ShowForTaskUid { get; set; }
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


