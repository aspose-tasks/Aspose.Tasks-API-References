---
title: PdfSaveOptions.DigitalSignatureDetails
second_title: Aspose.Tasks for .NET API Reference
description: PdfSaveOptions property. Gets or sets a digital signature details. If not set then no signing will be performed
type: docs
weight: 30
url: /net/aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails/
---
## PdfSaveOptions.DigitalSignatureDetails property

Gets or sets a digital signature details. If not set, then no signing will be performed.

```csharp
public PdfDigitalSignatureDetails DigitalSignatureDetails { get; set; }
```

## Examples

Shows how to set a digital signature details. If not set, then no signing will be performed.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
var certificate = new X509Certificate2();

// set a digital signature details. If not set, then no signing will be performed.
options.DigitalSignatureDetails = new PdfDigitalSignatureDetails(
    certificate,
    "reason",
    "location",
    new DateTime(2019, 1, 1),
    PdfDigitalSignatureHashAlgorithm.Sha1);

// tune additional properties
// set the <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> in which the document will be saved.
options.PresentationFormat = PresentationFormat.GanttChart;

// set a desired conformance level for generated PDF document
options.Compliance = PdfCompliance.PdfA1b;

project.Save(OutDir + "WorkWithDigitalSignatureDetails_out.pdf", options);
```

### See Also

* class [PdfDigitalSignatureDetails](../../pdfdigitalsignaturedetails/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


