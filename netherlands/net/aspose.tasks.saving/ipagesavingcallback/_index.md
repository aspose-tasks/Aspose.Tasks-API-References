---
title: "Interface IPageSavingCallback"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Saving.IPageSavingCallback interface. Vertegenwoordigt een callback die wordt aangeroepen wanneer elke pagina in een meerpagina-document wordt opgeslagen naar een aparte stream"
type: docs
weight: 2020
url: /nl/net/aspose.tasks.saving/ipagesavingcallback/
---
## IPageSavingCallback interface

Stelt een callback voor die wordt aangeroepen wanneer elke pagina in een meerpagina-document wordt opgeslagen naar een aparte stream.

```csharp
public interface IPageSavingCallback
```

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [OnFinish](../../aspose.tasks.saving/ipagesavingcallback/onfinish/)() | Methode die wordt aangeroepen wanneer alle pagina's zijn geschreven. |
| [PageSaving](../../aspose.tasks.saving/ipagesavingcallback/pagesaving/)(PageSavingArgs) | De methode die moet worden aangeroepen wanneer een pagina wordt opgeslagen in een stream. |

## Voorbeelden

Toont hoe een meerpagina-document kan worden opgeslagen naar door de gebruiker geleverde streams met behulp van een callback voor het opslaan van pagina's.

```csharp
[Test] 
public void UsePageSavingCallbackToSavePageToSeparateStreams()
{
    var project = new Project(DataDir + "Homemoveplan.mpp");

    var imageSaveOptions = new ImageSaveOptions(SaveFileFormat.Png);

    var callback = new CustomPageSavingCallback();
    imageSaveOptions.PageSavingCallback = callback;
    imageSaveOptions.RenderToSinglePage = false;
    project.Save(Stream.Null, imageSaveOptions);

    foreach (var streams in callback.PageStreams)
    {
        // verwerk elke paginastream
    }
}

private sealed class CustomPageSavingCallback : IPageSavingCallback
{
    public List<MemoryStream> PageStreams { get; } = new List<MemoryStream>();

    public void PageSaving(PageSavingArgs args)
    {
        var memoryStream = new MemoryStream();
        args.Stream = memoryStream;
        args.KeepStreamOpen = false;
        this.PageStreams.Add(memoryStream);
    }

    public void OnFinish()
    {
    }
}
```

### Zie ook

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


