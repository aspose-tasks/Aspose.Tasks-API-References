---
title: "Απαρίθμηση PdfCompliance"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Απαρίθμηση Aspose.Tasks.Saving.PdfCompliance. Καθορίζει το επίπεδο συμμόρφωσης PDF για το αρχείο εξόδου"
type: docs
weight: 2070
url: /el/net/aspose.tasks.saving/pdfcompliance/
---
## PdfCompliance enumeration

Καθορίζει το επίπεδο συμμόρφωσης PDF για το αρχείο εξόδου.

```csharp
public enum PdfCompliance
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Pdf15 | `0` | Επίπεδο συμμόρφωσης PDF/15. |
| PdfA1a | `1` | Επίπεδο συμμόρφωσης PDF/A-1a. |
| PdfA1b | `2` | Επίπεδο συμμόρφωσης PDF/A-1b. |

## Παραδείγματα

Δείχνει πώς να ορίσετε το επιθυμητό επίπεδο συμμόρφωσης για το παραγόμενο έγγραφο PDF.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();

// ορίστε το επιθυμητό επίπεδο συμμόρφωσης για το παραγόμενο έγγραφο PDF
// η προεπιλογή είναι τύπου <see cref=\"PdfCompliance.Pdf15\"/>
options.Compliance = PdfCompliance.PdfA1b;

// ρυθμίστε πρόσθετες ιδιότητες
// ορίστε το <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat\" /> στο οποίο θα αποθηκευτεί το έγγραφο.
options.PresentationFormat = PresentationFormat.GanttChart;

project.Save(OutDir + "WorkWithPdfCompliance_out.pdf", options);
```

### Δείτε επίσης

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


