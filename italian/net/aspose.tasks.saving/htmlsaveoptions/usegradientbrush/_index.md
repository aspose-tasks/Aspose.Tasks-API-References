---
title: "HtmlSaveOptions.UseGradientBrush"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "HtmlSaveOptions property. Ottiene o imposta un valore che indica se utilizzare il pennello gradiente durante il rendering del layout del progetto. Attualmente l'uso del pennello gradiente non è supportato durante il rendering in HTML"
type: docs
weight: 160
url: /it/net/aspose.tasks.saving/htmlsaveoptions/usegradientbrush/
---
## HtmlSaveOptions.UseGradientBrush property

Ottiene o imposta un valore che indica se utilizzare un pennello a gradiente durante il rendering del layout del progetto. Attualmente l'uso del pennello a gradiente non è supportato nel rendering in HTML.

```csharp
public override bool UseGradientBrush { get; set; }
```

## Esempi

Mostra come impostare un font personalizzato che verrà utilizzato per esportare il progetto in un file HTML.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new HtmlSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart,
                      FitContent = true
                  };

options.FontSettings.UseProjectDefaultFont = false;
options.FontSettings.DefaultFontName = "Segoe UI Black";
project.Save(OutDir + "AddDefaultFontDuringSavingAsHtml_out.html", options);
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


