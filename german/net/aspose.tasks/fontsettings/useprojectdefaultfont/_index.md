---
title: "FontSettings.UseProjectDefaultFont"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "FontSettings-Eigenschaft. Liest oder setzt einen Wert, der angibt, ob die Standardschriftart für das Rendern verwendet werden muss."
type: docs
weight: 40
url: /de/net/aspose.tasks/fontsettings/useprojectdefaultfont/
---
## FontSettings.UseProjectDefaultFont property

Ruft ab oder legt einen Wert fest, der angibt, ob die Standardschrift für das Rendern verwendet werden muss.

```csharp
public bool UseProjectDefaultFont { get; set; }
```

## Hinweise

Wenn der Wert False ist und DefaultFontName angegeben wird, verwendet die Rendering‑Engine die durch DefaultFontName angegebene Schriftart als Ersatzschriftart. Andernfalls werden 'Arial' (falls installiert) oder 'Generic Sans Serif'-Schriften als Ersatzschriftart verwendet. Die Ersatzschriftart wird beim Rendern der Projektansicht genutzt, wenn ein Textstil auf eine Schriftart verweist, die im aktuellen Betriebssystem nicht installiert ist. Für eine genauere Kontrolle der Schriftauflösung können Sie den [`FontResolveCallback`](../fontresolvecallback/)‑Callback verwenden.

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


