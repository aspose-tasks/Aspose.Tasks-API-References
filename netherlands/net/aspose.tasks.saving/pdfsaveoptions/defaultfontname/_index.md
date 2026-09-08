---
title: "DefaultFontName"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Haalt of stelt het standaard- of fallback-lettertype in voor weergave."
type: docs
weight: 30
url: /nl/net/aspose.tasks.saving/pdfsaveoptions/defaultfontname/
---
## PdfSaveOptions.DefaultFontName property

Haalt op of stelt het standaard‑ (of fallback‑)lettertype in voor weergave.

```csharp
public string DefaultFontName { get; set; }
```

### Voorbeelden

Toont hoe een aangepast lettertype in te stellen dat zal worden gebruikt voor het afdrukken van de uitvoer‑pdf.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart, FitContent = true, UseProjectDefaultFont = false, DefaultFontName = "Segoe UI Black"
                  };
project.Save(OutDir + "CreateProject2_out.pdf", options);
```

### Zie ook

* class [PdfSaveOptions](../../pdfsaveoptions)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor Aspose.Tasks.dll -->
