---
title: "SaveOptions.PageCount"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "SaveOptions eigenschap. Geeft of stelt het aantal pagina's van het project in."
type: docs
weight: 120
url: /nl/net/aspose.tasks.saving/saveoptions/pagecount/
---
## SaveOptions.PageCount property

Haalt op of stelt het aantal pagina's van het project in.

```csharp
public int PageCount { get; }
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

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


