---
title: "PdfSaveOptions.Pages"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà PdfSaveOptions. Ottiene o imposta l'elenco dei numeri di pagina da salvare quando il layout del progetto viene salvato in file separati. Tutte le pagine saranno salvate se questo elenco è vuoto"
type: docs
weight: 60
url: /it/net/aspose.tasks.saving/pdfsaveoptions/pages/
---
## PdfSaveOptions.Pages property

Ottiene o imposta l'elenco dei numeri di pagina da salvare quando il layout del progetto viene salvato in file separati. Tutte le pagine verranno salvate se questo elenco è vuoto.

```csharp
public List<int> Pages { get; set; }
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


