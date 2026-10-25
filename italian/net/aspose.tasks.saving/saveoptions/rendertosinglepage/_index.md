---
title: "SaveOptions.RenderToSinglePage"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà SaveOptions. Ottiene o imposta un valore che indica se un progetto deve essere renderizzato su una singola pagina quando viene salvato in formato grafico. La dimensione della pagina verrà modificata affinché il progetto renderizzato possa adattarsi a una pagina."
type: docs
weight: 150
url: /it/net/aspose.tasks.saving/saveoptions/rendertosinglepage/
---
## SaveOptions.RenderToSinglePage property

Ottiene o imposta un valore che indica se un progetto deve essere renderizzato su una singola pagina quando il progetto è salvato in formato grafico. La dimensione della pagina sarà modificata in modo che il progetto renderizzato possa adattarsi a una pagina.

```csharp
public bool RenderToSinglePage { get; set; }
```

## Esempi

Mostra come salvare le pagine selezionate di un progetto in un file PDF.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");
var options = new PdfSaveOptions();
options.RenderToSinglePage = false;
options.Pages = new List<int>();

// verifichiamo il numero di pagine che possono essere esportate
Console.WriteLine("Page Count: " + options.PageCount);

options.Pages.Add(1);
options.Pages.Add(4);
project.Save(OutDir + "SaveToMultiplePDFFiles_out.pdf", options);
```

Mostra come utilizzare la proprietà RenderToSinglePage per specificare che il progetto deve essere salvato in un PDF a una pagina.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
options.PresentationFormat = PresentationFormat.TaskUsage;
options.Timescale = Timescale.DefinedInView;
options.RenderToSinglePage = true;
options.StartDate = new DateTime(2012, 12, 22);
options.EndDate = new DateTime(2013, 05, 10);

project.Save(OutDir + "WorkWithRenderToSinglePage_out.pdf", options);
```

Mostra come salvare le pagine selezionate come immagine.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
                  {
                      RenderToSinglePage = false,
                      StartDate = project.Get(Prj.StartDate),
                      EndDate = project.Get(Prj.FinishDate),
                      PageSize = PageSize.Letter
                  };
options.Pages.Add(2);

project.Save(OutDir + "SaveSelectedPagesImageSaveOptions_page2_out.jpeg", options);
```

Mostra come salvare il layout in file separati.

```csharp
var project = new Project(DataDir + "Homemoveplan.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);
options.StartDate = project.Get(Prj.StartDate).AddDays(-3);
options.EndDate = project.Get(Prj.FinishDate);
options.MarkCriticalTasks = true;
options.LegendDrawingOptions = LegendDrawingOptions.NoLegend;
options.FontSettings.DefaultFontName = "Segoe UI Black";
options.FontSettings.UseProjectDefaultFont = false;
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

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


