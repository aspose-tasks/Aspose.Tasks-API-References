---
title: "DefaultFontName"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Ottiene o imposta il font predefinito o di riserva per il rendering."
type: docs
weight: 40
url: /it/net/aspose.tasks.saving/htmlsaveoptions/defaultfontname/
---
## HtmlSaveOptions.DefaultFontName property

Ottiene o imposta il carattere predefinito (o di riserva) per il rendering.

```csharp
public string DefaultFontName { get; set; }
```

### Esempi

Mostra come impostare un font personalizzato che verrà utilizzato per esportare il progetto in un file HTML.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new HtmlSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart,
                      FitContent = true,
                      UseProjectDefaultFont = false,
                      DefaultFontName = "Segoe UI Black"
                  };
project.Save(OutDir + "AddDefaultFontDuringSavingAsHtml_out.html", options);
```

### Vedi anche

* class [HtmlSaveOptions](../../htmlsaveoptions)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per Aspose.Tasks.dll -->
