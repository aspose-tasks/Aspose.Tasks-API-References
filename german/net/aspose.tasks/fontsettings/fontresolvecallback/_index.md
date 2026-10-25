---
title: "FontSettings.FontResolveCallback"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "FontSettings-Eigenschaft. Liest oder setzt einen Callback, der verwendet werden kann, um aufgelöste Schriften anzupassen."
type: docs
weight: 30
url: /de/net/aspose.tasks/fontsettings/fontresolvecallback/
---
## FontSettings.FontResolveCallback property

Ruft ab oder legt einen Rückruf fest, der verwendet werden kann, um aufgelöste Schriften anzupassen.

```csharp
public FontResolveCallbackDelegate FontResolveCallback { get; set; }
```

## Beispiele

Zeigt, wie man einen benutzerdefinierten Schriftauflösungs-Callback festlegt, um benutzerdefinierten Code auszuführen, der eine Ersatzschriftart festlegt oder die spezifische Schriftart ersetzt.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
};

options.FontSettings.FontResolveCallback = delegate(FontResolveEventArgs args)
{
    if (args.RequestedFontName != args.ResolvedFontName)
    {
        // Sieht so aus, als könnte die genaue Schriftart nicht gefunden werden und eine Ersatzschriftart wurde festgelegt.
        // Wir können die Ersatzschriftart überschreiben.
        args.ResolvedFontName = "Arial";
    }

    // Oder einfach die spezifische Schriftart ersetzen:
    if (args.RequestedFontName == "Comic Sans MS")
    {
        args.ResolvedFontName = "Arial";
    }
};

project.Save(OutDir + "EstimatedMilestoneTasks_out3.pdf", options);
```

### Siehe auch

* delegate [FontResolveCallbackDelegate](../../fontresolvecallbackdelegate/)
* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


