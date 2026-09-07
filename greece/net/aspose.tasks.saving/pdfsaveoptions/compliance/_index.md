---
title: "PdfSaveOptions.Compliance"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PdfSaveOptions. Λαμβάνει ή ορίζει το επιθυμητό επίπεδο συμμόρφωσης για το παραγόμενο έγγραφο PDF. Η προεπιλογή είναι Pdf15."
type: docs
weight: 20
url: /el/net/aspose.tasks.saving/pdfsaveoptions/compliance/
---
## PdfSaveOptions.Compliance property

Λαμβάνει ή ορίζει το επιθυμητό επίπεδο συμμόρφωσης για το παραγόμενο έγγραφο PDF. Η προεπιλογή είναι Pdf15.

```csharp
public PdfCompliance Compliance { get; set; }
```

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

* enum [PdfCompliance](../../pdfcompliance/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


