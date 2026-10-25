---
title: "IPageSavingCallback.PageSaving"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "IPageSavingCallback-methode. De methode die wordt aangeroepen wanneer een pagina naar een stream wordt opgeslagen"
type: docs
weight: 20
url: /nl/net/aspose.tasks.saving/ipagesavingcallback/pagesaving/
---
## IPageSavingCallback.PageSaving method

De methode die moet worden aangeroepen wanneer een pagina wordt opgeslagen in een stream.

```csharp
public void PageSaving(PageSavingArgs args)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| args | PageSavingArgs | De argumenten voor het opslaan van de pagina. |

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

* class [PageSavingArgs](../../pagesavingargs/)
* interface [IPageSavingCallback](../)
* namespace [Aspose.Tasks.Saving](../../ipagesavingcallback/)
* assembly [Aspose.Tasks](../../../)


