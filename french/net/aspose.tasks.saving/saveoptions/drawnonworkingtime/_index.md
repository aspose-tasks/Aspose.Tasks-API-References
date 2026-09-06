---
title: "SaveOptions.DrawNonWorkingTime"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété SaveOptions. Obtient ou définit une valeur indiquant si le temps non travaillé doit être dessiné. La valeur par défaut est TRUE."
type: docs
weight: 30
url: /fr/net/aspose.tasks.saving/saveoptions/drawnonworkingtime/
---
## SaveOptions.DrawNonWorkingTime property

Obtient ou définit une valeur indiquant si le temps non travaillé doit être dessiné (la valeur par défaut est TRUE).

```csharp
public bool DrawNonWorkingTime { get; set; }
```

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


