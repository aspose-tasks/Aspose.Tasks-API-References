---
title: "FontResolveCallback"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Ottiene o imposta un callback che può essere usato per personalizzare i caratteri risolti."
type: docs
weight: 90
url: /it/net/aspose.tasks.saving/htmlsaveoptions/fontresolvecallback/
---
## HtmlSaveOptions.FontResolveCallback property

Ottiene o imposta un callback che può essere usato per personalizzare i caratteri risolti.

```csharp
public FontResolveCallbackDelegate FontResolveCallback { get; set; }
```

### Esempi

Mostra come impostare un callback di risoluzione dei font personalizzato per eseguire codice definito dall'utente per impostare un font di fallback o sostituire un font specifico.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
    FontResolveCallback = delegate(FontResolveEventArgs args)
    {
        if (args.RequestedFontName != args.ResolvedFontName)
        {
            // Sembra che il font esatto non possa essere trovato e sia stato impostato il font di fallback.
            // Possiamo sovrascrivere il font di fallback.
            args.ResolvedFontName = "Arial";
        }

        // Oppure semplicemente sostituire il font specifico:
        if (args.RequestedFontName == "Comic Sans MS")
        {
            args.ResolvedFontName = "Arial";
        }
    }
};

project.Save(OutDir + "EstimatedMilestoneTasks_out3.pdf", options);
```

### Vedi anche

* delegate [FontResolveCallbackDelegate](../../../aspose.tasks/fontresolvecallbackdelegate)
* class [HtmlSaveOptions](../../htmlsaveoptions)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per Aspose.Tasks.dll -->
