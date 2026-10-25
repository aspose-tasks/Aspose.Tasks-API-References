---
title: "FontResolveCallback"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Haalt op of stelt een callback in die kan worden gebruikt om opgeloste lettertypen aan te passen."
type: docs
weight: 30
url: /nl/net/aspose.tasks.saving/imagesaveoptions/fontresolvecallback/
---
## ImageSaveOptions.FontResolveCallback property

Haalt op of stelt een callback in die kan worden gebruikt om opgeloste lettertypen aan te passen.

```csharp
public FontResolveCallbackDelegate FontResolveCallback { get; set; }
```

### Voorbeelden

Toont hoe een aangepaste lettertype‑oplossingscallback in te stellen om gebruikersgedefinieerde code uit te voeren om een fallback‑lettertype in te stellen of om het specifieke lettertype te vervangen.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
    FontResolveCallback = delegate(FontResolveEventArgs args)
    {
        if (args.RequestedFontName != args.ResolvedFontName)
        {
            // Het lijkt erop dat het exacte lettertype niet kan worden gevonden en er een fallback‑lettertype is ingesteld.
            // We kunnen het fallback‑lettertype overschrijven.
            args.ResolvedFontName = "Arial";
        }

        // Of vervang simpelweg het specifieke lettertype:
        if (args.RequestedFontName == "Comic Sans MS")
        {
            args.ResolvedFontName = "Arial";
        }
    }
};

project.Save(OutDir + "EstimatedMilestoneTasks_out3.pdf", options);
```

### Zie ook

* delegate [FontResolveCallbackDelegate](../../../aspose.tasks/fontresolvecallbackdelegate)
* class [ImageSaveOptions](../../imagesaveoptions)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor Aspose.Tasks.dll -->
