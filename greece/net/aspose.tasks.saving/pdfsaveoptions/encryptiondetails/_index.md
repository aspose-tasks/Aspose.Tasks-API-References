---
title: "PdfSaveOptions.EncryptionDetails"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PdfSaveOptions. Λαμβάνει ή ορίζει λεπτομέρειες κρυπτογράφησης. Εάν δεν οριστεί, δεν θα γίνει κρυπτογράφηση."
type: docs
weight: 40
url: /el/net/aspose.tasks.saving/pdfsaveoptions/encryptiondetails/
---
## PdfSaveOptions.EncryptionDetails property

Λαμβάνει ή ορίζει λεπτομέρειες κρυπτογράφησης. Εάν δεν οριστεί, δεν θα γίνει κρυπτογράφηση.

```csharp
public PdfEncryptionDetails EncryptionDetails { get; set; }
```

## Παραδείγματα

Δείχνει πώς να ορίσετε λεπτομέρειες κρυπτογράφησης εγγράφου PDF. Εάν δεν οριστεί, δεν θα γίνει κρυπτογράφηση.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var encryptionDetails = new PdfEncryptionDetails("userPassword", "ownerPassword", PdfEncryptionAlgorithm.RC4_128);

var options = new PdfSaveOptions();

// Ορίστε λεπτομέρειες κρυπτογράφησης εγγράφου PDF.
options.EncryptionDetails = encryptionDetails;

// ρυθμίστε πρόσθετες ιδιότητες
// ορίστε το <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat\" /> στο οποίο θα αποθηκευτεί το έγγραφο.
options.PresentationFormat = PresentationFormat.GanttChart;

project.Save(OutDir + "WorkWithEncryptionDetails_out.pdf", options);
```

### Δείτε επίσης

* class [PdfEncryptionDetails](../../pdfencryptiondetails/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


