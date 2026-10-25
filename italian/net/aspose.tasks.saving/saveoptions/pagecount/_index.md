---
title: "SaveOptions.PageCount"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà SaveOptions. Ottiene o imposta il numero di pagine del progetto"
type: docs
weight: 120
url: /it/net/aspose.tasks.saving/saveoptions/pagecount/
---
## SaveOptions.PageCount property

Ottiene o imposta il numero di pagine del progetto.

```csharp
public int PageCount { get; }
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

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


