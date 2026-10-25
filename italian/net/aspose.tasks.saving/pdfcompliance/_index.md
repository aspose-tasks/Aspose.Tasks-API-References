---
title: "Enum PdfCompliance"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.Saving.PdfCompliance. Specifica il livello di conformità PDF per il file di output"
type: docs
weight: 2070
url: /it/net/aspose.tasks.saving/pdfcompliance/
---
## PdfCompliance enumeration

Specifica il livello di conformità PDF per il file di output.

```csharp
public enum PdfCompliance
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Pdf15 | `0` | Livello di conformità PDF/15. |
| PdfA1a | `1` | Livello di conformità PDF/A-1a. |
| PdfA1b | `2` | Livello di conformità PDF/A-1b. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


