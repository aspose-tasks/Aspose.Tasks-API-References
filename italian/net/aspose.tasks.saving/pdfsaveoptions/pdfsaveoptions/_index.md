---
title: "PdfSaveOptions.PdfSaveOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "PdfSaveOptions costruttore. Inizializza una nuova istanza della classe PdfSaveOptions che può essere usata per salvare un documento nel formato PDF"
type: docs
weight: 10
url: /it/net/aspose.tasks.saving/pdfsaveoptions/pdfsaveoptions/
---
## PdfSaveOptions constructor

Inizializza una nuova istanza della classe [`PdfSaveOptions`](../) che può essere usata per salvare un documento nel formato [`PDF`](../../savefileformat/).

```csharp
public PdfSaveOptions()
```

## Esempi

Mostra come salvare le pagine selezionate di un progetto in un file PDF.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");
var options = new PdfSaveOptions();
options.RenderToSinglePage = false;
options.Pages = new List<int>();

// verifichiamo il numero di pagine che possono essere esportate
Console.WriteLine("Page Count: " + options.PageCount);

options.Pages.Add(1);
options.Pages.Add(4);
project.Save(OutDir + "SaveToMultiplePDFFiles_out.pdf", options);
```

### Vedi anche

* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


