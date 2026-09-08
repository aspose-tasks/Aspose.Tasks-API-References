---
title: "SaveOptions.CustomPageSize"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "SaveOptions-eigenschap. Haalt de aangepaste paginagrootte op of stelt deze in in punten (1 punt = 1/72 inch)."
type: docs
weight: 20
url: /nl/net/aspose.tasks.saving/saveoptions/custompagesize/
---
## SaveOptions.CustomPageSize property

Haalt op of stelt de aangepaste paginagrootte in punten in (1 punt = 1/72 inch).

```csharp
public SizeF CustomPageSize { get; set; }
```

## Voorbeelden

Toont hoe de aangepaste paginagrootte in te stellen wanneer het project wordt opgeslagen als PDF.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
options.PresentationFormat = PresentationFormat.GanttChart;
options.CustomPageSize = new SizeF(5.8F * 72, 8.3F * 72);

project.Save(OutDir + "WorkWithCustomPageSize_out.pdf", options);
```

### Zie ook

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


