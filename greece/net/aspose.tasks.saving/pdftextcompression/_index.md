---
title: "Απαρίθμηση PdfTextCompression"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Saving.PdfTextCompression enum. Καθορίζει έναν τύπο συμπίεσης που εφαρμόζεται σε όλο το περιεχόμενο του αρχείου PDF εκτός από τις εικόνες."
type: docs
weight: 2140
url: /el/net/aspose.tasks.saving/pdftextcompression/
---
## PdfTextCompression enumeration

Καθορίζει έναν τύπο συμπίεσης που εφαρμόζεται σε όλο το περιεχόμενο του αρχείου PDF εκτός από τις εικόνες.

```csharp
public enum PdfTextCompression
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| None | `0` | Χωρίς συμπίεση. |
| Flate | `1` | Συμπίεση Flate. |

## Παραδείγματα

Δείχνει πώς να ορίσετε έναν τύπο συμπίεσης που θα χρησιμοποιείται για όλες τις ροές περιεχομένου εκτός από τις εικόνες.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();

// ορίστε τον τύπο συμπίεσης που θα χρησιμοποιείται για όλες τις ροές περιεχομένου εκτός από τις εικόνες
options.TextCompression = PdfTextCompression.Flate;

// ρυθμίστε πρόσθετες ιδιότητες
// ορίστε το <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat\" /> στο οποίο θα αποθηκευτεί το έγγραφο.
options.PresentationFormat = PresentationFormat.GanttChart;

// ορίστε το επιθυμητό επίπεδο συμμόρφωσης για το παραγόμενο έγγραφο PDF
options.Compliance = PdfCompliance.PdfA1b;

project.Save(OutDir + "WorkWithTextCompression_out.pdf", options);
```

### Δείτε επίσης

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


