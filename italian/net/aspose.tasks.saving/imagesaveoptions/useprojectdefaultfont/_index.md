---
title: "UseProjectDefaultFont"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Ottiene o imposta un valore che indica se il carattere predefinito deve essere usato per il rendering."
type: docs
weight: 110
url: /it/net/aspose.tasks.saving/imagesaveoptions/useprojectdefaultfont/
---
## ImageSaveOptions.UseProjectDefaultFont property

Ottiene o imposta un valore che indica se il carattere predefinito deve essere usato per il rendering.

```csharp
public bool UseProjectDefaultFont { get; set; }
```

### Osservazioni

Quando il valore è False e DefaultFontName è specificato, il motore di rendering utilizzerà il carattere specificato da DefaultFontName come carattere di riserva. Altrimenti vengono utilizzati come carattere di riserva 'Arial' (se installato) o i caratteri 'Generic Sans Serif'. Il carattere di riserva viene utilizzato durante il rendering della vista del progetto quando uno stile di testo fa riferimento a un carattere non installato sul sistema operativo corrente. Per un maggiore controllo sulla risoluzione dei caratteri è possibile utilizzare il callback [`FontResolveCallback`](../fontresolvecallback).

### Esempi

Mostra come salvare il layout in file separati.

```csharp
var project = new Project(DataDir + "Homemoveplan.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);
options.StartDate = project.Get(Prj.StartDate).AddDays(-3);
options.EndDate = project.Get(Prj.FinishDate);
options.MarkCriticalTasks = true;
options.DefaultFontName = "Segoe UI Black";
options.UseProjectDefaultFont = false;
options.PageSize = PageSize.Letter;

options.Gridlines = new List<Gridline>();

var gridline = new Gridline { GridlineType = GridlineType.GanttRow, Color = Color.CornflowerBlue, Pattern = LinePattern.Dashed };
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles1_out.png", options);

// Salva il layout del progetto in file separati
options.RenderToSinglePage = false;
project.Save(OutDir + "PrintProjectPagesToSeparateFiles2_out.png", options);
```

### Vedi anche

* class [ImageSaveOptions](../../imagesaveoptions)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per Aspose.Tasks.dll -->
