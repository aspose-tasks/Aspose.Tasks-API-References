---
title: "PdfSaveOptions.TextCompression"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PdfSaveOptions. Λαμβάνει ή ορίζει έναν τύπο συμπίεσης που θα χρησιμοποιηθεί για όλες τις ροές περιεχομένου εκτός από εικόνες. Η προεπιλογή είναι Flate"
type: docs
weight: 100
url: /el/net/aspose.tasks.saving/pdfsaveoptions/textcompression/
---
## PdfSaveOptions.TextCompression property

Λαμβάνει ή ορίζει τύπο συμπίεσης που θα χρησιμοποιηθεί για όλες τις ροές περιεχομένου εκτός από τις εικόνες. Η προεπιλογή είναι Flate.

```csharp
public PdfTextCompression TextCompression { get; set; }
```

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

* enum [PdfTextCompression](../../pdftextcompression/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


