---
title: "PdfSaveOptions.TextCompression"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PdfSaveOptions-eigenschap. Haalt een compressietype op of stelt dit in dat wordt gebruikt voor alle inhoudsstromen behalve afbeeldingen. Standaard is Flate"
type: docs
weight: 100
url: /nl/net/aspose.tasks.saving/pdfsaveoptions/textcompression/
---
## PdfSaveOptions.TextCompression property

Haalt op of stelt een compressietype in dat moet worden gebruikt voor alle content‑streams behalve afbeeldingen. Standaard is Flate.

```csharp
public PdfTextCompression TextCompression { get; set; }
```

## Voorbeelden

Toont hoe een compressietype in te stellen dat wordt gebruikt voor alle contentstreams, behalve afbeeldingen.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();

// stel compressietype in dat wordt gebruikt voor alle contentstreams, behalve afbeeldingen
options.TextCompression = PdfTextCompression.Flate;

// stuur extra eigenschappen af
// stel de <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat\" /> in waarin het document wordt opgeslagen.
options.PresentationFormat = PresentationFormat.GanttChart;

// stel een gewenst conformiteitsniveau in voor het gegenereerde PDF‑document
options.Compliance = PdfCompliance.PdfA1b;

project.Save(OutDir + "WorkWithTextCompression_out.pdf", options);
```

### Zie ook

* enum [PdfTextCompression](../../pdftextcompression/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


