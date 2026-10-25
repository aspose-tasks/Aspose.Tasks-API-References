---
title: "GanttBarStyle.ShowForCategories"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "GanttBarStyle proprietà. Ottiene o imposta le categorie di attività per le quali lo stile è applicato. È applicabile per gli stili genitore o comuni delle barre nel diagramma di Gantt, vedi BarStyles"
type: docs
weight: 200
url: /it/net/aspose.tasks.visualization/ganttbarstyle/showforcategories/
---
## GanttBarStyle.ShowForCategories property

Ottiene o imposta le categorie di attività per le quali lo stile è applicato. È applicabile per gli stili genitore (o comuni) delle barre nel diagramma di Gantt (vedi [`BarStyles`](../../../aspose.tasks/ganttchartview/barstyles/)).

```csharp
public IList<GanttBarShowFor> ShowForCategories { get; set; }
```

## Esempi

Mostra come utilizzare le categorie ShowFor.

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

// lavorare con il progetto...
```

### Vedi anche

* enum [GanttBarShowFor](../../ganttbarshowfor/)
* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


