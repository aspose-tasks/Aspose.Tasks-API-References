---
title: "Enum GanttBarSize"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.GanttBarSize enum. Spécifie la hauteur d'une barre en points"
type: docs
weight: 700
url: /fr/net/aspose.tasks/ganttbarsize/
---
## GanttBarSize enumeration

Spécifie la hauteur d'une barre en points.

```csharp
public enum GanttBarSize
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| BarSize6 | `0` | Taille de la barre 6 points. |
| BarSize8 | `1` | Taille de la barre 8 points. |
| BarSize10 | `2` | Taille de la barre 10 points. |
| BarSize12 | `3` | Taille de la barre 12 points. |
| BarSize14 | `4` | Taille de la barre 14 points. |
| BarSize18 | `5` | Taille de la barre 18 points. |
| BarSize24 | `6` | Taille de la barre 24 points. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


