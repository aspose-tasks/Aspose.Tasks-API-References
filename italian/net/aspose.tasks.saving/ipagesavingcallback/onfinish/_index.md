---
title: "IPageSavingCallback.OnFinish"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "IPageSavingCallback metodo. Metodo che verrà chiamato quando tutte le pagine sono state scritte"
type: docs
weight: 10
url: /it/net/aspose.tasks.saving/ipagesavingcallback/onfinish/
---
## IPageSavingCallback.OnFinish method

Metodo che verrà chiamato quando tutte le pagine sono state scritte.

```csharp
public void OnFinish()
```

## Esempi

Mostra come salvare un documento multipagina in flussi forniti dall'utente utilizzando il callback di salvataggio della pagina.

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
        // elabora ogni flusso di pagina
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

### Vedi anche

* interface [IPageSavingCallback](../)
* namespace [Aspose.Tasks.Saving](../../ipagesavingcallback/)
* assembly [Aspose.Tasks](../../../)


