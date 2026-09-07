---
title: "PdfSaveOptions.PdfSaveOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής PdfSaveOptions. Αρχικοποιεί μια νέα παρουσία της κλάσης PdfSaveOptions που μπορεί να χρησιμοποιηθεί για την αποθήκευση ενός εγγράφου σε μορφή PDF"
type: docs
weight: 10
url: /el/net/aspose.tasks.saving/pdfsaveoptions/pdfsaveoptions/
---
## PdfSaveOptions constructor

Αρχικοποιεί μια νέα παρουσία της κλάσης [`PdfSaveOptions`](../) που μπορεί να χρησιμοποιηθεί για την αποθήκευση ενός εγγράφου σε μορφή [`PDF`](../../savefileformat/).

```csharp
public PdfSaveOptions()
```

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε επιλεγμένες σελίδες ενός έργου σε αρχείο PDF.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");
var options = new PdfSaveOptions();
options.RenderToSinglePage = false;
options.Pages = new List<int>();

// ας ελέγξουμε τον αριθμό των σελίδων που μπορούν να εξαχθούν
Console.WriteLine("Page Count: " + options.PageCount);

options.Pages.Add(1);
options.Pages.Add(4);
project.Save(OutDir + "SaveToMultiplePDFFiles_out.pdf", options);
```

### Δείτε επίσης

* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


