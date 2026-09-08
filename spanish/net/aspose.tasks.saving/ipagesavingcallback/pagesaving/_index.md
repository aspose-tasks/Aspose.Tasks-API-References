---
title: "IPageSavingCallback.PageSaving"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método IPageSavingCallback. El método que se llamará cuando una página se guarde en un flujo"
type: docs
weight: 20
url: /es/net/aspose.tasks.saving/ipagesavingcallback/pagesaving/
---
## IPageSavingCallback.PageSaving method

El método que se debe llamar cuando una página se guarda en un flujo.

```csharp
public void PageSaving(PageSavingArgs args)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| args | PageSavingArgs | Los argumentos de guardado de página. |

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

* class [PageSavingArgs](../../pagesavingargs/)
* interface [IPageSavingCallback](../)
* namespace [Aspose.Tasks.Saving](../../ipagesavingcallback/)
* assembly [Aspose.Tasks](../../../)


