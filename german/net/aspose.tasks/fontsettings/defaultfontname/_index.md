---
title: "FontSettings.DefaultFontName"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "FontSettings-Eigenschaft. Liest oder setzt die Standard- oder Ersatzschriftart für das Rendern."
type: docs
weight: 20
url: /de/net/aspose.tasks/fontsettings/defaultfontname/
---
## FontSettings.DefaultFontName property

Ruft ab oder legt die Standard‑ (oder Ersatz‑)Schrift für das Rendern fest.

```csharp
public string DefaultFontName { get; set; }
```

## Beispiele

Zeigt, wie man eine benutzerdefinierte Schriftart festlegt, die für den Druck des Ausgabe‑PDFs verwendet wird.

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

### Siehe auch

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


