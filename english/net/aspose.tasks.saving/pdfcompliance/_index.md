---
title: Enum PdfCompliance
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Saving.PdfCompliance enum. Specifies the PDF compliance level to output file
type: docs
weight: 2010
url: /net/aspose.tasks.saving/pdfcompliance/
---
## PdfCompliance enumeration

Specifies the PDF compliance level to output file.

```csharp
public enum PdfCompliance
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Pdf15 | `0` | PDF/15 level of compliance. |
| PdfA1a | `1` | PDF/A-1a level of compliance. |
| PdfA1b | `2` | PDF/A-1b level of compliance. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


