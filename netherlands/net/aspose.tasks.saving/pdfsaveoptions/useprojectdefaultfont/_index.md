---
title: "UseProjectDefaultFont"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Haalt op of stelt een waarde in die aangeeft of het standaardlettertype moet worden gebruikt voor weergave."
type: docs
weight: 120
url: /nl/net/aspose.tasks.saving/pdfsaveoptions/useprojectdefaultfont/
---
## PdfSaveOptions.UseProjectDefaultFont property

Haalt op of stelt een waarde in die aangeeft of het standaardlettertype moet worden gebruikt voor weergave.

```csharp
public bool UseProjectDefaultFont { get; set; }
```

### Opmerkingen

Wanneer de waarde False is en DefaultFontName is opgegeven, zal de renderengine het door DefaultFontName gespecificeerde lettertype gebruiken als fallback-lettertype. Anders worden 'Arial' (indien geïnstalleerd) of 'Generic Sans Serif' lettertypen gebruikt als fallback-lettertype. Het fallback-lettertype wordt gebruikt tijdens het renderen van de projectweergave wanneer een tekststijl verwijst naar een lettertype dat niet op het huidige besturingssysteem is geïnstalleerd. Voor meer controle over lettertype‑resolutie kun je de [`FontResolveCallback`](../fontresolvecallback) callback gebruiken.

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
