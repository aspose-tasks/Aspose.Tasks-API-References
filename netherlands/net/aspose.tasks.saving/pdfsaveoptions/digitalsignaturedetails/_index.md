---
title: "PdfSaveOptions.DigitalSignatureDetails"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PdfSaveOptions-eigenschap. Haalt op of stelt digitale handtekeningdetails in. Indien niet ingesteld, wordt er geen ondertekening uitgevoerd."
type: docs
weight: 30
url: /nl/net/aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails/
---
## PdfSaveOptions.DigitalSignatureDetails property

Haalt op of stelt details van een digitale handtekening in. Indien niet ingesteld, wordt er geen ondertekening uitgevoerd.

```csharp
public PdfDigitalSignatureDetails DigitalSignatureDetails { get; set; }
```

## Voorbeelden

Toont hoe digitale handtekeningdetails in te stellen. Indien niet ingesteld, wordt er geen ondertekening uitgevoerd.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
var certificate = new X509Certificate2();

// Stel digitale handtekeningdetails in. Indien niet ingesteld, wordt er geen ondertekening uitgevoerd.
options.DigitalSignatureDetails = new PdfDigitalSignatureDetails(
    certificate,
    "reason",
    "location",
    new DateTime(2019, 1, 1),
    PdfDigitalSignatureHashAlgorithm.Sha1);

// stuur extra eigenschappen af
// stel de <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat\" /> in waarin het document wordt opgeslagen.
options.PresentationFormat = PresentationFormat.GanttChart;

// stel een gewenst conformiteitsniveau in voor het gegenereerde PDF‑document
options.Compliance = PdfCompliance.PdfA1b;

project.Save(OutDir + "WorkWithDigitalSignatureDetails_out.pdf", options);
```

### Zie ook

* class [PdfDigitalSignatureDetails](../../pdfdigitalsignaturedetails/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


