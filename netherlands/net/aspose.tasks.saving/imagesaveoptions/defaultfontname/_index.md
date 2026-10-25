---
title: "DefaultFontName"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Haalt of stelt het standaard- of fallback-lettertype in voor weergave."
type: docs
weight: 20
url: /nl/net/aspose.tasks.saving/imagesaveoptions/defaultfontname/
---
## ImageSaveOptions.DefaultFontName property

Haalt op of stelt het standaard‑ (of fallback‑)lettertype in voor weergave.

```csharp
public string DefaultFontName { get; set; }
```

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
