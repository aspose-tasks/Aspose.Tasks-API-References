---
title: "PdfSaveOptions.Pages"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PdfSaveOptions-eigenschap. Haalt op of stelt de lijst met paginanummers in die moeten worden opgeslagen bij het opslaan van de projectlay-out naar afzonderlijke bestanden. Alle pagina's worden opgeslagen als deze lijst leeg is."
type: docs
weight: 60
url: /nl/net/aspose.tasks.saving/pdfsaveoptions/pages/
---
## PdfSaveOptions.Pages property

Haalt op of stelt de lijst met paginanummers in die moeten worden opgeslagen bij het opslaan van de projectlay-out naar afzonderlijke bestanden. Alle pagina's worden opgeslagen als deze lijst leeg is.

```csharp
public List<int> Pages { get; set; }
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


