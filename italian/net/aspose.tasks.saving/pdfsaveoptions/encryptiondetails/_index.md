---
title: "PdfSaveOptions.EncryptionDetails"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà PdfSaveOptions. Ottiene o imposta i dettagli della crittografia. Se non impostati, non verrà eseguita alcuna crittografia."
type: docs
weight: 40
url: /it/net/aspose.tasks.saving/pdfsaveoptions/encryptiondetails/
---
## PdfSaveOptions.EncryptionDetails property

Ottiene o imposta i dettagli della crittografia. Se non impostato, non verrà eseguita alcuna crittografia.

```csharp
public PdfEncryptionDetails EncryptionDetails { get; set; }
```

## Esempi

Mostra come impostare i dettagli della crittografia di un documento PDF. Se non impostati, non verrà eseguita alcuna crittografia.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var encryptionDetails = new PdfEncryptionDetails("userPassword", "ownerPassword", PdfEncryptionAlgorithm.RC4_128);

var options = new PdfSaveOptions();

// imposta i dettagli della crittografia di un documento PDF
options.EncryptionDetails = encryptionDetails;

// regola proprietà aggiuntive
// imposta il <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> in cui il documento verrà salvato.
options.PresentationFormat = PresentationFormat.GanttChart;

project.Save(OutDir + "WorkWithEncryptionDetails_out.pdf", options);
```

### Vedi anche

* class [PdfEncryptionDetails](../../pdfencryptiondetails/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


