---
title: "Enum PdfCompliance"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Saving.PdfCompliance enum. Specificeert het PDF-conformiteitsniveau voor het uitvoerbestand"
type: docs
weight: 2070
url: /nl/net/aspose.tasks.saving/pdfcompliance/
---
## PdfCompliance enumeration

Bepaalt het PDF-conformiteitsniveau voor het uitvoerbestand.

```csharp
public enum PdfCompliance
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Pdf15 | `0` | PDF/15-conformiteitsniveau. |
| PdfA1a | `1` | PDF/A-1a-conformiteitsniveau. |
| PdfA1b | `2` | PDF/A-1b-conformiteitsniveau. |

## Voorbeelden

Toont hoe een gewenst conformiteitsniveau in te stellen voor een gegenereerd PDF-document.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();

// stel een gewenst conformiteitsniveau in voor het gegenereerde PDF‑document
// standaard is <see cref="PdfCompliance.Pdf15"/> type
options.Compliance = PdfCompliance.PdfA1b;

// stuur extra eigenschappen af
// stel de <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat\" /> in waarin het document wordt opgeslagen.
options.PresentationFormat = PresentationFormat.GanttChart;

project.Save(OutDir + "WorkWithPdfCompliance_out.pdf", options);
```

### Zie ook

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


