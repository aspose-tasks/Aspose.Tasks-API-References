---
title: "GanttBarStyle.ShowForTaskUid"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "GanttBarStyle proprietà. Ottiene o imposta l'Id univoco di un'attività per la quale lo stile è applicato. È applicabile per stili specifici dell'attività delle barre nel diagramma di Gantt, vedi CustomBarStyles"
type: docs
weight: 210
url: /it/net/aspose.tasks.visualization/ganttbarstyle/showfortaskuid/
---
## GanttBarStyle.ShowForTaskUid property

Ottiene o imposta l'Id univoco di un'attività per la quale lo stile è applicato. È applicabile per stili specifici dell'attività delle barre nel diagramma di Gantt (vedi [`CustomBarStyles`](../../../aspose.tasks/ganttchartview/custombarstyles/)).

```csharp
public int? ShowForTaskUid { get; set; }
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


