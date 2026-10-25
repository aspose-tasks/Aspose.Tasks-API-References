---
title: "IPageSavingCallback.OnFinish"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método IPageSavingCallback. Método que se llamará cuando se hayan escrito todas las páginas"
type: docs
weight: 10
url: /es/net/aspose.tasks.saving/ipagesavingcallback/onfinish/
---
## IPageSavingCallback.OnFinish method

Método que será llamado cuando se escriban todas las páginas.

```csharp
public void OnFinish()
```

## Ejemplos

Muestra cómo guardar un documento multipágina en flujos proporcionados por el usuario usando la devolución de llamada de guardado de página.

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
        // procesar cada flujo de página
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

### Ver también

* interface [IPageSavingCallback](../)
* namespace [Aspose.Tasks.Saving](../../ipagesavingcallback/)
* assembly [Aspose.Tasks](../../../)


