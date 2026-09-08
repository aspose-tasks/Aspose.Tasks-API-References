---
title: "Enum PdfTextCompression"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Saving.PdfTextCompression enum. Specificeert een type compressie dat wordt toegepast op alle inhoud in het PDF‑bestand, behalve afbeeldingen."
type: docs
weight: 2140
url: /nl/net/aspose.tasks.saving/pdftextcompression/
---
## PdfTextCompression enumeration

Bepaalt een type compressie dat wordt toegepast op alle inhoud in het PDF-bestand, behalve afbeeldingen.

```csharp
public enum PdfTextCompression
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| None | `0` | Geen compressie. |
| Flate | `1` | Flate-compressie. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


