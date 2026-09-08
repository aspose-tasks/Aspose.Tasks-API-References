---
title: "PdfSaveOptions.PdfSaveOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PdfSaveOptions-constructor. Initialiseert een nieuw exemplaar van de PdfSaveOptions‑klasse die kan worden gebruikt om een document op te slaan in PDF‑formaat"
type: docs
weight: 10
url: /nl/net/aspose.tasks.saving/pdfsaveoptions/pdfsaveoptions/
---
## PdfSaveOptions constructor

Initialiseert een nieuw exemplaar van de [`PdfSaveOptions`](../) klasse die kan worden gebruikt om een document op te slaan in het [`PDF`](../../savefileformat/) formaat.

```csharp
public PdfSaveOptions()
```

## Voorbeelden

Toont hoe geselecteerde pagina's van een project kunnen worden opgeslagen in een PDF‑bestand.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");
var options = new PdfSaveOptions();
options.RenderToSinglePage = false;
options.Pages = new List<int>();

// laten we controleren hoeveel pagina's kunnen worden geëxporteerd
Console.WriteLine("Page Count: " + options.PageCount);

options.Pages.Add(1);
options.Pages.Add(4);
project.Save(OutDir + "SaveToMultiplePDFFiles_out.pdf", options);
```

### Zie ook

* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


