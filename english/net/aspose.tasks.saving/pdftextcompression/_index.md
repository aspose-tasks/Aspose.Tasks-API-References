---
title: Enum PdfTextCompression
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Saving.PdfTextCompression enum. Specifies a type of compression applied to all content in the PDF file except images
type: docs
weight: 2110
url: /net/aspose.tasks.saving/pdftextcompression/
---
## PdfTextCompression enumeration

Specifies a type of compression applied to all content in the PDF file except images.

```csharp
public enum PdfTextCompression
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No compression. |
| Flate | `1` | Flate compression. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


