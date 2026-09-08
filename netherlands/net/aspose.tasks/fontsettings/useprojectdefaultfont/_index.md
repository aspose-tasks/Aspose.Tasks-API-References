---
title: "FontSettings.UseProjectDefaultFont"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "FontSettings eigenschap. Haalt een waarde op of stelt deze in die aangeeft of het standaardlettertype moet worden gebruikt voor het renderen"
type: docs
weight: 40
url: /nl/net/aspose.tasks/fontsettings/useprojectdefaultfont/
---
## FontSettings.UseProjectDefaultFont property

Haalt op of stelt een waarde in die aangeeft of het standaardlettertype moet worden gebruikt voor weergave.

```csharp
public bool UseProjectDefaultFont { get; set; }
```

## Opmerkingen

Wanneer de waarde False is en DefaultFontName is opgegeven, zal de renderengine het lettertype gebruiken dat door DefaultFontName is gespecificeerd als fallback-lettertype. Anders worden 'Arial' (indien geïnstalleerd) of 'Generic Sans Serif' lettertypen gebruikt als fallback-lettertype. Het fallback-lettertype wordt gebruikt tijdens het renderen van de projectweergave wanneer een tekststijl verwijst naar een lettertype dat niet op het huidige besturingssysteem is geïnstalleerd. Voor meer controle over lettertype‑resolutie kun je de [`FontResolveCallback`](../fontresolvecallback/) callback gebruiken.

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


