---
title: "UseProjectDefaultFont"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Haalt op of stelt een waarde in die aangeeft of het standaardlettertype moet worden gebruikt voor weergave."
type: docs
weight: 110
url: /nl/net/aspose.tasks.saving/imagesaveoptions/useprojectdefaultfont/
---
## ImageSaveOptions.UseProjectDefaultFont property

Haalt op of stelt een waarde in die aangeeft of het standaardlettertype moet worden gebruikt voor weergave.

```csharp
public bool UseProjectDefaultFont { get; set; }
```

### Opmerkingen

Wanneer de waarde False is en DefaultFontName is opgegeven, zal de renderengine het door DefaultFontName gespecificeerde lettertype gebruiken als fallback-lettertype. Anders worden 'Arial' (indien geïnstalleerd) of 'Generic Sans Serif' lettertypen gebruikt als fallback-lettertype. Het fallback-lettertype wordt gebruikt tijdens het renderen van de projectweergave wanneer een tekststijl verwijst naar een lettertype dat niet op het huidige besturingssysteem is geïnstalleerd. Voor meer controle over lettertype‑resolutie kun je de [`FontResolveCallback`](../fontresolvecallback) callback gebruiken.

### Voorbeelden

Toont hoe de lay‑out op te slaan in afzonderlijke bestanden.

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

// Projectlay-out opslaan in afzonderlijke bestanden
options.RenderToSinglePage = false;
project.Save(OutDir + "PrintProjectPagesToSeparateFiles2_out.png", options);
```

### Zie ook

* class [ImageSaveOptions](../../imagesaveoptions)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor Aspose.Tasks.dll -->
