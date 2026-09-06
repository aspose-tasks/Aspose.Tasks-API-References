---
title: "GanttChartView.ShowBarSplits"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété GanttChartView. Obtient ou définit une valeur indiquant si les divisions de tâches sur le Gantt Chart doivent être affichées"
type: docs
weight: 140
url: /fr/net/aspose.tasks/ganttchartview/showbarsplits/
---
## GanttChartView.ShowBarSplits property

Obtient ou définit une valeur indiquant si les découpages de tâches sur le Gantt Chart doivent être affichés.

```csharp
public bool ShowBarSplits { get; set; }
```

## Exemples

Montre comment définir certaines propriétés utiles de la vue du diagramme de Gantt.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// définir une valeur indiquant si les barres sont arrondies au jour le plus proche
view.BarRounding = false;
// définir la hauteur, en points, des barres Gantt dans le diagramme de Gantt
view.BarSize = GanttBarSize.BarSize24;
// définir une valeur indiquant si les barres de regroupement seront masquées lors de l'expansion de la tâche récapitulative
view.HideRollupBarsWhenSummaryExpanded = true;
// définir la couleur du temps non travaillé
view.NonWorkingTimeColor = Color.Azure;
// définir une valeur indiquant si les barres du diagramme de Gantt doivent être regroupées
view.RollUpGanttBars = true;
// définir une valeur indiquant si les découpages de tâches sur le diagramme de Gantt doivent être affichés
view.ShowBarSplits = true;
// définir une valeur indiquant si les dessins sur le diagramme de Gantt doivent être affichés
view.ShowDrawings = true;
// définir un pourcentage pour réduire ou agrandir l'espacement entre les unités sur le niveau de l'échelle de temps
view.TimescaleSizePercentage = 10;

project.Save(OutDir + "WorkWithGanttChartViews_out.pdf", SaveFileFormat.Pdf);
```

### Voir aussi

* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


