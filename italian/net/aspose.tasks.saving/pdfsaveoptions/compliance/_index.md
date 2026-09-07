---
title: "PdfSaveOptions.Compliance"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà PdfSaveOptions. Ottiene o imposta il livello di conformità desiderato per il documento PDF generato. Il valore predefinito è Pdf15"
type: docs
weight: 20
url: /it/net/aspose.tasks.saving/pdfsaveoptions/compliance/
---
## PdfSaveOptions.Compliance property

Ottiene o imposta il livello di conformità desiderato per il documento PDF generato. Il valore predefinito è Pdf15.

```csharp
public PdfCompliance Compliance { get; set; }
```

## Esempi

Mostra come impostare un livello di conformità desiderato per il documento PDF generato.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();

// imposta un livello di conformità desiderato per il documento PDF generato
// Il valore predefinito è <see cref="PdfCompliance.Pdf15"/> tipo
options.Compliance = PdfCompliance.PdfA1b;

// regola proprietà aggiuntive
// imposta il <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> in cui il documento verrà salvato.
options.PresentationFormat = PresentationFormat.GanttChart;

project.Save(OutDir + "WorkWithPdfCompliance_out.pdf", options);
```

### Vedi anche

* enum [PdfCompliance](../../pdfcompliance/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


