---
title: "FontSettings.DefaultFontName"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà FontSettings. Ottiene o imposta il font predefinito o di fallback per il rendering"
type: docs
weight: 20
url: /it/net/aspose.tasks/fontsettings/defaultfontname/
---
## FontSettings.DefaultFontName property

Ottiene o imposta il carattere predefinito (o di riserva) per il rendering.

```csharp
public string DefaultFontName { get; set; }
```

## Esempi

Mostra come impostare un font personalizzato che verrà usato per la stampa del PDF di output.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart, FitContent = true
                  };

options.FontSettings.UseProjectDefaultFont = false;
options.FontSettings.DefaultFontName = "Segoe UI Black";
project.Save(OutDir + "CreateProject2_out.pdf", options);
```

### Vedi anche

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


