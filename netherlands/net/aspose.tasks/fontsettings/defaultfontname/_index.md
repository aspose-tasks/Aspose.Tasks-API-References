---
title: "FontSettings.DefaultFontName"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "FontSettings eigenschap. Haalt het standaard‑ of fallback‑lettertype op of stelt dit in voor het renderen"
type: docs
weight: 20
url: /nl/net/aspose.tasks/fontsettings/defaultfontname/
---
## FontSettings.DefaultFontName property

Haalt op of stelt het standaard‑ (of fallback‑)lettertype in voor weergave.

```csharp
public string DefaultFontName { get; set; }
```

## Voorbeelden

Toont hoe een aangepast lettertype in te stellen dat zal worden gebruikt voor het afdrukken van de uitvoer‑pdf.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart, FitContent = true
                  };

options.FontSettings.UseProjectDefaultFont = false;
options.FontSettings.DefaultFontName = "Segoe UI Black";
project.Save(OutDir + "CreateProject2_out.pdf", options);
```

### Zie ook

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


