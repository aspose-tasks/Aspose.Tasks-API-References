---
title: "PdfSaveOptions.Compliance"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PdfSaveOptions-eigenschap. Haalt op of stelt een gewenst conformiteitsniveau in voor het gegenereerde PDF-document. Standaard is Pdf15."
type: docs
weight: 20
url: /nl/net/aspose.tasks.saving/pdfsaveoptions/compliance/
---
## PdfSaveOptions.Compliance property

Haalt op of stelt een gewenst conformiteitsniveau in voor het gegenereerde PDF‑document. Standaard is Pdf15.

```csharp
public PdfCompliance Compliance { get; set; }
```

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

* enum [PdfCompliance](../../pdfcompliance/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


