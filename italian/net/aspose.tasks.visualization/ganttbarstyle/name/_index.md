---
title: "GanttBarStyle.Name"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "GanttBarStyle proprietà. Ottiene o imposta un nome dello stile"
type: docs
weight: 150
url: /it/net/aspose.tasks.visualization/ganttbarstyle/name/
---
## GanttBarStyle.Name property

Ottiene o imposta un nome dello stile.

```csharp
public string Name { get; set; }
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

* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


