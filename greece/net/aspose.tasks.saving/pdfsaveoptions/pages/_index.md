---
title: "PdfSaveOptions.Pages"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PdfSaveOptions. Λαμβάνει ή ορίζει τη λίστα αριθμών σελίδων που θα αποθηκευτούν όταν αποθηκεύεται η διάταξη του έργου σε ξεχωριστά αρχεία. Όλες οι σελίδες θα αποθηκευτούν εάν αυτή η λίστα είναι κενή."
type: docs
weight: 60
url: /el/net/aspose.tasks.saving/pdfsaveoptions/pages/
---
## PdfSaveOptions.Pages property

Λαμβάνει ή ορίζει τη λίστα αριθμών σελίδων που θα αποθηκευτούν όταν αποθηκεύεται η διάταξη του έργου σε ξεχωριστά αρχεία. Όλες οι σελίδες θα αποθηκευτούν εάν αυτή η λίστα είναι κενή.

```csharp
public List<int> Pages { get; set; }
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


