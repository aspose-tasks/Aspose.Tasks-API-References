---
title: "IPageSavingCallback.OnFinish"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode IPageSavingCallback. Méthode qui sera appelée lorsque toutes les pages sont écrites"
type: docs
weight: 10
url: /fr/net/aspose.tasks.saving/ipagesavingcallback/onfinish/
---
## IPageSavingCallback.OnFinish method

Méthode qui sera appelée lorsque toutes les pages sont écrites.

```csharp
public void OnFinish()
```

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

* interface [IPageSavingCallback](../)
* namespace [Aspose.Tasks.Saving](../../ipagesavingcallback/)
* assembly [Aspose.Tasks](../../../)


