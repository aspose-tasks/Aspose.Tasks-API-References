---
title: "HtmlSaveOptions.UseGradientBrush"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "HtmlSaveOptions eigenschap. Haalt een waarde op of stelt deze in die aangeeft of een gradientborstel moet worden gebruikt bij het renderen van de projectlay-out. Het gebruik van een gradientborstel wordt momenteel niet ondersteund bij het renderen naar HTML."
type: docs
weight: 160
url: /nl/net/aspose.tasks.saving/htmlsaveoptions/usegradientbrush/
---
## HtmlSaveOptions.UseGradientBrush property

Haalt op of stelt een waarde in die aangeeft of een gradient‑kwast moet worden gebruikt bij het renderen van de projectlay-out. Het gebruik van een gradient‑kwast wordt momenteel niet ondersteund bij het renderen naar HTML.

```csharp
public override bool UseGradientBrush { get; set; }
```

## Voorbeelden

Toont hoe een aangepast lettertype in te stellen dat wordt gebruikt om het project te exporteren naar een HTML‑bestand.

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

### Zie ook

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


