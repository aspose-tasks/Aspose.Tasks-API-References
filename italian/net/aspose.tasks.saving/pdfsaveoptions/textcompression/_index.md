---
title: "PdfSaveOptions.TextCompression"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "PdfSaveOptions proprietà. Ottiene o imposta un tipo di compressione da utilizzare per tutti i flussi di contenuto eccetto le immagini. Il valore predefinito è Flate"
type: docs
weight: 100
url: /it/net/aspose.tasks.saving/pdfsaveoptions/textcompression/
---
## PdfSaveOptions.TextCompression property

Ottiene o imposta il tipo di compressione da utilizzare per tutti i flussi di contenuto eccetto le immagini. Il valore predefinito è Flate.

```csharp
public PdfTextCompression TextCompression { get; set; }
```

## Esempi

Mostra come impostare un tipo di compressione da utilizzare per tutti i flussi di contenuto, eccetto le immagini.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();

// imposta il tipo di compressione da utilizzare per tutti i flussi di contenuto, eccetto le immagini
options.TextCompression = PdfTextCompression.Flate;

// regola proprietà aggiuntive
// imposta il <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> in cui il documento verrà salvato.
options.PresentationFormat = PresentationFormat.GanttChart;

// imposta un livello di conformità desiderato per il documento PDF generato
options.Compliance = PdfCompliance.PdfA1b;

project.Save(OutDir + "WorkWithTextCompression_out.pdf", options);
```

### Vedi anche

* enum [PdfTextCompression](../../pdftextcompression/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


