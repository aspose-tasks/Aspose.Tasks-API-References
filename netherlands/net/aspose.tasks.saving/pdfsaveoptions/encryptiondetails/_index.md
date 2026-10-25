---
title: "PdfSaveOptions.EncryptionDetails"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PdfSaveOptions-eigenschap. Haalt op of stelt encryptiedetails in. Indien niet ingesteld, wordt er geen versleuteling uitgevoerd."
type: docs
weight: 40
url: /nl/net/aspose.tasks.saving/pdfsaveoptions/encryptiondetails/
---
## PdfSaveOptions.EncryptionDetails property

Haalt op of stelt encryptiedetails in. Indien niet ingesteld, wordt er geen encryptie uitgevoerd.

```csharp
public PdfEncryptionDetails EncryptionDetails { get; set; }
```

## Voorbeelden

Toont hoe encryptiedetails van een PDF-document in te stellen. Indien niet ingesteld, wordt er geen versleuteling uitgevoerd.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var encryptionDetails = new PdfEncryptionDetails("userPassword", "ownerPassword", PdfEncryptionAlgorithm.RC4_128);

var options = new PdfSaveOptions();

// Stel encryptiedetails van een PDF-document in.
options.EncryptionDetails = encryptionDetails;

// stuur extra eigenschappen af
// stel de <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat\" /> in waarin het document wordt opgeslagen.
options.PresentationFormat = PresentationFormat.GanttChart;

project.Save(OutDir + "WorkWithEncryptionDetails_out.pdf", options);
```

### Zie ook

* class [PdfEncryptionDetails](../../pdfencryptiondetails/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


