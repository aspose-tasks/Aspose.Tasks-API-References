---
title: "DefaultFontName"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Ottiene o imposta il font predefinito o di riserva per il rendering."
type: docs
weight: 30
url: /it/net/aspose.tasks.saving/pdfsaveoptions/defaultfontname/
---
## PdfSaveOptions.DefaultFontName property

Ottiene o imposta il carattere predefinito (o di riserva) per il rendering.

```csharp
public string DefaultFontName { get; set; }
```

### Esempi

Mostra come impostare un font personalizzato che verrà usato per la stampa del PDF di output.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart, FitContent = true, UseProjectDefaultFont = false, DefaultFontName = "Segoe UI Black"
                  };
project.Save(OutDir + "CreateProject2_out.pdf", options);
```

### Vedi anche

* class [PdfSaveOptions](../../pdfsaveoptions)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per Aspose.Tasks.dll -->
