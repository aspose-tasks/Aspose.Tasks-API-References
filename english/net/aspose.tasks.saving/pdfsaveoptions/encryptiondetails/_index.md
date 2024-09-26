---
title: PdfSaveOptions.EncryptionDetails
second_title: Aspose.Tasks for .NET API Reference
description: PdfSaveOptions property. Gets or sets a encryption details. If not set then no encryption will be performed
type: docs
weight: 40
url: /net/aspose.tasks.saving/pdfsaveoptions/encryptiondetails/
---
## PdfSaveOptions.EncryptionDetails property

Gets or sets a encryption details. If not set, then no encryption will be performed.

```csharp
public PdfEncryptionDetails EncryptionDetails { get; set; }
```

## Examples

Shows how to set a encryption details of PDF document. If not set, then no encryption will be performed.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var encryptionDetails = new PdfEncryptionDetails("userPassword", "ownerPassword", PdfEncryptionAlgorithm.RC4_128);

var options = new PdfSaveOptions();

// set a encryption details of PDF document
options.EncryptionDetails = encryptionDetails;

// tune additional properties
// set the <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> in which the document will be saved.
options.PresentationFormat = PresentationFormat.GanttChart;

project.Save(OutDir + "WorkWithEncryptionDetails_out.pdf", options);
```

### See Also

* class [PdfEncryptionDetails](../../pdfencryptiondetails/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


