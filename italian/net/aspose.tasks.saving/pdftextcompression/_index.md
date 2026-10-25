---
title: "Enum PdfTextCompression"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.Saving.PdfTextCompression enum. Specifica un tipo di compressione applicata a tutti i contenuti nel file PDF, eccetto le immagini."
type: docs
weight: 2140
url: /it/net/aspose.tasks.saving/pdftextcompression/
---
## PdfTextCompression enumeration

Specifica un tipo di compressione applicata a tutti i contenuti del file PDF, eccetto le immagini.

```csharp
public enum PdfTextCompression
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Nessuna compressione. |
| Flate | `1` | Compressione Flate. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


