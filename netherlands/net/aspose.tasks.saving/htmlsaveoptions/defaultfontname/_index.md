---
title: "DefaultFontName"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Haalt of stelt het standaard- of fallback-lettertype in voor weergave."
type: docs
weight: 40
url: /nl/net/aspose.tasks.saving/htmlsaveoptions/defaultfontname/
---
## HtmlSaveOptions.DefaultFontName property

Haalt op of stelt het standaard‑ (of fallback‑)lettertype in voor weergave.

```csharp
public string DefaultFontName { get; set; }
```

### Voorbeelden

Toont hoe een aangepast lettertype in te stellen dat wordt gebruikt om het project te exporteren naar een HTML‑bestand.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new HtmlSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart,
                      FitContent = true,
                      UseProjectDefaultFont = false,
                      DefaultFontName = "Segoe UI Black"
                  };
project.Save(OutDir + "AddDefaultFontDuringSavingAsHtml_out.html", options);
```

### Zie ook

* class [HtmlSaveOptions](../../htmlsaveoptions)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor Aspose.Tasks.dll -->
