---
title: "SaveOptions.MarkCriticalTasks"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété SaveOptions. Obtient ou définit une valeur indiquant si les tâches critiques doivent être affichées en couleur rouge. La valeur par défaut est FALSE."
type: docs
weight: 100
url: /fr/net/aspose.tasks.saving/saveoptions/markcriticaltasks/
---
## SaveOptions.MarkCriticalTasks property

Obtient ou définit une valeur indiquant si les tâches critiques doivent être affichées en rouge (la valeur par défaut est FALSE).

```csharp
public bool MarkCriticalTasks { get; set; }
```

## Exemples

Montre comment imprimer les tâches critiques lors de l'enregistrement aux formats d'image.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png)
{
    StartDate = project.Get(Prj.StartDate).AddDays(-3),
    EndDate = project.Get(Prj.FinishDate),
    MarkCriticalTasks = true,
    LegendDrawingOptions = LegendDrawingOptions.NoLegend,
    Gridlines = new List<Gridline>()
};

var gridline = new Gridline { GridlineType = GridlineType.GanttRow, Color = Color.CornflowerBlue, Pattern = LinePattern.Dashed };
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles1_out.png", options);

// Enregistrer la mise en page du projet dans des fichiers séparés
options.RenderToSinglePage = false;
project.Save(OutDir + "PrintProjectPagesToSeparateFiles2_out.png", options);
```

### Voir aussi

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


