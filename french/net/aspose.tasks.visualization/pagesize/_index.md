---
title: "Énumération PageSize"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Visualization.PageSize enum. Spécifie la taille de la page."
type: docs
weight: 3250
url: /fr/net/aspose.tasks.visualization/pagesize/
---
## PageSize enumeration

Spécifie la taille de la page.

```csharp
public enum PageSize
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Letter | `0` | La taille de la page Letter en points est 792 × 612. |
| Ledger | `1` | La taille de la page Ledger en points est 1224 × 792. |
| A0 | `2` | La taille de la page A0 en points est 3371 × 2384. |
| A1 | `3` | La taille de la page A1 en points est 2384 × 1685. |
| A2 | `4` | La taille de la page A2 en points est 1684 × 1190. |
| A3 | `5` | La taille de la page A3 en points est 1190 × 842. |
| A4 | `6` | La taille de la page A4 en points est 842 × 595. |
| DefinedInView | `7` | Utilisez la taille de page définie dans la vue [`PageSettings`](../pagesettings/) (View.PageInfo.PageSettings). |

## Exemples

Montre comment définir une valeur indiquant que les sous‑tâches sur la barre de tâche récapitulative doivent être agrégées.

```csharp
var project = new Project(DataDir + "Project2.mpp");

project.DisplayOptions.ShowProjectSummaryTask = true;
project.Set(Prj.ShowProjectSummaryTask, true);

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
    FitContent = true,
    RollUpGanttBars = true,

    // OU
    // options.RollUpGanttBars = false;
    // DrawNonWorkingTime = true,
    PageSize = PageSize.A3
};

project.Save(OutDir + "RenderGanttChartWithBarsRolledUp_out.pdf", options);
```

### Voir aussi

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


