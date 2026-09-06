---
title: "SaveOptions.RollUpGanttBars"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété SaveOptions. Obtient ou définit une valeur indiquant si les sous‑tâches sur la barre de tâche récapitulative doivent être marquées. Pour les sous‑tâches, le champ Rollup indique si les informations des barres Gantt des sous‑tâches seront agrégées dans la barre de tâche récapitulative. Pour les tâches récapitulatives, le champ Rollup indique si la barre de tâche récapitulative affiche les barres agrégées. Vous devez définir le champ Rollup des tâches récapitulatives sur Oui pour que les sous‑tâches puissent être agrégées."
type: docs
weight: 160
url: /fr/net/aspose.tasks.saving/saveoptions/rollupganttbars/
---
## SaveOptions.RollUpGanttBars property

Obtient ou définit une valeur indiquant si les sous‑tâches sur la barre de tâche récapitulative doivent être marquées. Pour les sous‑tâches, le champ Rollup indique si les informations des barres Gantt des sous‑tâches seront agrégées dans la barre de tâche récapitulative. Pour les tâches récapitulatives, le champ Rollup indique si la barre de tâche récapitulative affiche les barres agrégées. Vous devez définir le champ Rollup des tâches récapitulatives sur Oui pour que les sous‑tâches puissent être agrégées.

```csharp
public bool RollUpGanttBars { get; set; }
```

## Remarques

Ne s'applique que lorsque la vue du diagramme de Gantt est rendue.

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

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


