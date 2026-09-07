---
title: "SaveOptions.CustomPageSize"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà SaveOptions. Ottiene o imposta la dimensione personalizzata della pagina in punti (1 punto = 1/72 di pollice)."
type: docs
weight: 20
url: /it/net/aspose.tasks.saving/saveoptions/custompagesize/
---
## SaveOptions.CustomPageSize property

Ottiene o imposta la dimensione della pagina personalizzata in punti (1 punto = 1/72 di pollice).

```csharp
public SizeF CustomPageSize { get; set; }
```

## Esempi

Mostra come impostare la dimensione personalizzata della pagina quando il progetto viene salvato in PDF.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
options.PresentationFormat = PresentationFormat.GanttChart;
options.CustomPageSize = new SizeF(5.8F * 72, 8.3F * 72);

project.Save(OutDir + "WorkWithCustomPageSize_out.pdf", options);
```

### Vedi anche

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


