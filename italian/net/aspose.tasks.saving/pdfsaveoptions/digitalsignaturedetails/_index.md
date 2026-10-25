---
title: "PdfSaveOptions.DigitalSignatureDetails"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà PdfSaveOptions. Ottiene o imposta i dettagli della firma digitale. Se non impostati, non verrà eseguita alcuna firma."
type: docs
weight: 30
url: /it/net/aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails/
---
## PdfSaveOptions.DigitalSignatureDetails property

Ottiene o imposta i dettagli della firma digitale. Se non impostato, non verrà eseguita alcuna firma.

```csharp
public PdfDigitalSignatureDetails DigitalSignatureDetails { get; set; }
```

## Esempi

Mostra come impostare i dettagli della firma digitale. Se non impostati, non verrà eseguita alcuna firma.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
var certificate = new X509Certificate2();

// imposta i dettagli della firma digitale. Se non impostati, non verrà eseguita alcuna firma.
options.DigitalSignatureDetails = new PdfDigitalSignatureDetails(
    certificate,
    "reason",
    "location",
    new DateTime(2019, 1, 1),
    PdfDigitalSignatureHashAlgorithm.Sha1);

// regola proprietà aggiuntive
// imposta il <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> in cui il documento verrà salvato.
options.PresentationFormat = PresentationFormat.GanttChart;

// imposta un livello di conformità desiderato per il documento PDF generato
options.Compliance = PdfCompliance.PdfA1b;

project.Save(OutDir + "WorkWithDigitalSignatureDetails_out.pdf", options);
```

### Vedi anche

* class [PdfDigitalSignatureDetails](../../pdfdigitalsignaturedetails/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


