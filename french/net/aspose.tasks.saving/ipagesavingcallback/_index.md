---
title: "Interface IPageSavingCallback"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Saving.IPageSavingCallback interface. Représente un rappel qui est appelé lorsque chaque page d'un document multipage est enregistrée dans un flux séparé"
type: docs
weight: 2020
url: /fr/net/aspose.tasks.saving/ipagesavingcallback/
---
## IPageSavingCallback interface

Représente un rappel qui est appelé lorsque chaque page d'un document multipage est enregistrée dans un flux séparé.

```csharp
public interface IPageSavingCallback
```

## Méthodes

| Nom | Description |
| --- | --- |
| [OnFinish](../../aspose.tasks.saving/ipagesavingcallback/onfinish/)() | Méthode qui sera appelée lorsque toutes les pages sont écrites. |
| [PageSaving](../../aspose.tasks.saving/ipagesavingcallback/pagesaving/)(PageSavingArgs) | La méthode à appeler lorsqu’une page est enregistrée dans un flux. |

## Exemples

Montre comment enregistrer un document multipage dans des flux fournis par l'utilisateur en utilisant le rappel d'enregistrement de page.

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
        // traiter chaque flux de page
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

### Voir aussi

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


