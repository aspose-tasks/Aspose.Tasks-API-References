---
title: PdfSaveOptions.Compliance
second_title: Aspose.Tasks for .NET API Reference
description: PdfSaveOptions property. Gets or sets a desired compliance level for generated PDF document. Default is Pdf15
type: docs
weight: 20
url: /net/aspose.tasks.saving/pdfsaveoptions/compliance/
---
## PdfSaveOptions.Compliance property

Gets or sets a desired compliance level for generated PDF document. Default is Pdf15.

```csharp
public PdfCompliance Compliance { get; set; }
```

## Examples

Shows how to set a desired compliance level for generated PDF document.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();

// set a desired conformance level for generated PDF document
// default is <see cref="PdfCompliance.Pdf15"/> type
options.Compliance = PdfCompliance.PdfA1b;

// tune additional properties
// set the <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> in which the document will be saved.
options.PresentationFormat = PresentationFormat.GanttChart;

project.Save(OutDir + "WorkWithPdfCompliance_out.pdf", options);
```

### See Also

* enum [PdfCompliance](../../pdfcompliance/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


