---
title: "PdfSaveOptions.DigitalSignatureDetails"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PdfSaveOptions. Λαμβάνει ή ορίζει λεπτομέρειες ψηφιακής υπογραφής. Εάν δεν οριστεί, δεν θα γίνει υπογραφή."
type: docs
weight: 30
url: /el/net/aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails/
---
## PdfSaveOptions.DigitalSignatureDetails property

Λαμβάνει ή ορίζει λεπτομέρειες ψηφιακής υπογραφής. Εάν δεν οριστεί, δεν θα γίνει υπογραφή.

```csharp
public PdfDigitalSignatureDetails DigitalSignatureDetails { get; set; }
```

## Παραδείγματα

Δείχνει πώς να ορίσετε λεπτομέρειες ψηφιακής υπογραφής. Εάν δεν οριστεί, δεν θα γίνει υπογραφή.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
var certificate = new X509Certificate2();

// Ορίστε λεπτομέρειες ψηφιακής υπογραφής. Εάν δεν οριστεί, δεν θα γίνει υπογραφή.
options.DigitalSignatureDetails = new PdfDigitalSignatureDetails(
    certificate,
    "reason",
    "location",
    new DateTime(2019, 1, 1),
    PdfDigitalSignatureHashAlgorithm.Sha1);

// ρυθμίστε πρόσθετες ιδιότητες
// ορίστε το <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat\" /> στο οποίο θα αποθηκευτεί το έγγραφο.
options.PresentationFormat = PresentationFormat.GanttChart;

// ορίστε το επιθυμητό επίπεδο συμμόρφωσης για το παραγόμενο έγγραφο PDF
options.Compliance = PdfCompliance.PdfA1b;

project.Save(OutDir + "WorkWithDigitalSignatureDetails_out.pdf", options);
```

### Δείτε επίσης

* class [PdfDigitalSignatureDetails](../../pdfdigitalsignaturedetails/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


