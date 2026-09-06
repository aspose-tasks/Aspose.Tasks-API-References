---
title: "IPageSavingCallback.PageSaving"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode IPageSavingCallback. La méthode à appeler lorsqu'une page est enregistrée dans un flux"
type: docs
weight: 20
url: /fr/net/aspose.tasks.saving/ipagesavingcallback/pagesaving/
---
## IPageSavingCallback.PageSaving method

La méthode à appeler lorsqu’une page est enregistrée dans un flux.

```csharp
public void PageSaving(PageSavingArgs args)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| args | PageSavingArgs | Les arguments d'enregistrement de la page. |

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

* class [PageSavingArgs](../../pagesavingargs/)
* interface [IPageSavingCallback](../)
* namespace [Aspose.Tasks.Saving](../../ipagesavingcallback/)
* assembly [Aspose.Tasks](../../../)


