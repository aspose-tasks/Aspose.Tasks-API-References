---
title: "Enum TimescaleFitBehavior"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Enum Aspose.Tasks.Visualization.TimescaleFitBehavior. Représente un comportement utilisé pour aligner la zone d'échelle de temps avec la largeur de la page"
type: docs
weight: 3440
url: /fr/net/aspose.tasks.visualization/timescalefitbehavior/
---
## TimescaleFitBehavior enumeration

Représente un comportement utilisé pour aligner la zone de l'échelle de temps avec la largeur de la page.

```csharp
public enum TimescaleFitBehavior
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| DefinedInView | `0` | La section du calendrier est rendue selon la propriété View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage de la vue rendue. |
| NoScaleToEndDate | `1` | La section du calendrier est rendue exactement jusqu'à EndDate, même s'il y a un espace vide sur une page. |
| NoScaleToEndOfPage | `2` | La section du calendrier est rendue jusqu'à la fin (côté droit) de la dernière page. Ainsi, la dernière date rendue peut dépasser EndDate. |
| ScaleToEndOfPage | `3` | Le moteur de rendu tentera d'aligner les dates afin qu'EndDate soit aligné avec la fin (côté droit) de la dernière page. Correspond à l'option "Mise en page \ Vue \ Adapter l'échelle de temps à la fin de la page" de MS Project activée. |

## Exemples

Montre comment utiliser TimescaleFitBehavior pour faire en sorte que l'échelle de temps du diagramme de Gantt s'adapte à la fin de la dernière page.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.DefaultView as GanttChartView;

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.A4;
saveOptions.StartDate = project.StartDate;
saveOptions.EndDate = project.FinishDate;
saveOptions.ViewSettings = view;
saveOptions.TimescaleFitBehavior = TimescaleFitBehavior.ScaleToEndOfPage;

project.Save(OutDir + "WorkWithPageSizeDefinedInView_out.pdf", saveOptions);
```

### Voir aussi

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


