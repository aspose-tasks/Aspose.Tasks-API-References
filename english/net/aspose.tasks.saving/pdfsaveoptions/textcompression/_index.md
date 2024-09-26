---
title: PdfSaveOptions.TextCompression
second_title: Aspose.Tasks for .NET API Reference
description: PdfSaveOptions property. Gets or sets a compression type to be used for all content streams except images. Default is Flate
type: docs
weight: 100
url: /net/aspose.tasks.saving/pdfsaveoptions/textcompression/
---
## PdfSaveOptions.TextCompression property

Gets or sets a compression type to be used for all content streams except images. Default is Flate.

```csharp
public PdfTextCompression TextCompression { get; set; }
```

## Examples

Shows how to set a compression type to be used for all content streams except images.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();

// set compression type to be used for all content streams except images
options.TextCompression = PdfTextCompression.Flate;

// tune additional properties
// set the <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> in which the document will be saved.
options.PresentationFormat = PresentationFormat.GanttChart;

// set a desired conformance level for generated PDF document
options.Compliance = PdfCompliance.PdfA1b;

project.Save(OutDir + "WorkWithTextCompression_out.pdf", options);
```

### See Also

* enum [PdfTextCompression](../../pdftextcompression/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


