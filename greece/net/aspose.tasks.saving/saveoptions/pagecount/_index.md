---
title: "SaveOptions.PageCount"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα SaveOptions. Λαμβάνει ή ορίζει τον αριθμό των σελίδων του έργου"
type: docs
weight: 120
url: /el/net/aspose.tasks.saving/saveoptions/pagecount/
---
## SaveOptions.PageCount property

Αποκτά ή ορίζει τον αριθμό των σελίδων του έργου.

```csharp
public int PageCount { get; }
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

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


