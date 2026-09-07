---
title: "Interface IPageSavingCallback"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Interfaccia Aspose.Tasks.Saving.IPageSavingCallback. Rappresenta una callback che viene chiamata quando ogni pagina di un documento multipagina viene salvata in un flusso separato"
type: docs
weight: 2020
url: /it/net/aspose.tasks.saving/ipagesavingcallback/
---
## IPageSavingCallback interface

Rappresenta un callback che viene chiamato quando ogni pagina di un documento multipagina viene salvata in un flusso separato.

```csharp
public interface IPageSavingCallback
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [OnFinish](../../aspose.tasks.saving/ipagesavingcallback/onfinish/)() | Metodo che verrà chiamato quando tutte le pagine sono state scritte. |
| [PageSaving](../../aspose.tasks.saving/ipagesavingcallback/pagesaving/)(PageSavingArgs) | Il metodo da chiamare quando una pagina viene salvata in un flusso. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


