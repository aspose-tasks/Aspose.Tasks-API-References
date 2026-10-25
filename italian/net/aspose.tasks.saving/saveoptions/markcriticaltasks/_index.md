---
title: "SaveOptions.MarkCriticalTasks"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà SaveOptions. Ottiene o imposta un valore che indica se le attività critiche devono essere visualizzate in colore rosso. Il valore predefinito è FALSE."
type: docs
weight: 100
url: /it/net/aspose.tasks.saving/saveoptions/markcriticaltasks/
---
## SaveOptions.MarkCriticalTasks property

Ottiene o imposta un valore che indica se le attività critiche devono essere visualizzate in colore rosso (Il valore predefinito è FALSE).

```csharp
public bool MarkCriticalTasks { get; set; }
```

## Esempi

Mostra come stampare le attività critiche durante il salvataggio nei formati di file immagine.

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

// Salva il layout del progetto in file separati
options.RenderToSinglePage = false;
project.Save(OutDir + "PrintProjectPagesToSeparateFiles2_out.png", options);
```

### Vedi anche

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


