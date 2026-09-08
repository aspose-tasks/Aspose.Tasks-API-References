---
title: "Interfaz IPageSavingCallback"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.Saving.IPageSavingCallback interfaz. Representa una devolución de llamada que se invoca cuando cada página en un documento multipágina se guarda en un flujo separado"
type: docs
weight: 2020
url: /es/net/aspose.tasks.saving/ipagesavingcallback/
---
## IPageSavingCallback interface

Representa una devolución de llamada que se invoca cuando cada página de un documento multipágina se guarda en un flujo separado.

```csharp
public interface IPageSavingCallback
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| [OnFinish](../../aspose.tasks.saving/ipagesavingcallback/onfinish/)() | Método que será llamado cuando se escriban todas las páginas. |
| [PageSaving](../../aspose.tasks.saving/ipagesavingcallback/pagesaving/)(PageSavingArgs) | El método que se debe llamar cuando una página se guarda en un flujo. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


