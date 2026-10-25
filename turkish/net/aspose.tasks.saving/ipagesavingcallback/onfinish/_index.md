---
title: "IPageSavingCallback.OnFinish"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "IPageSavingCallback yöntemi. Tüm sayfalar yazıldığında çağrılacak yöntem"
type: docs
weight: 10
url: /tr/net/aspose.tasks.saving/ipagesavingcallback/onfinish/
---
## IPageSavingCallback.OnFinish method

Tüm sayfalar yazıldığında çağrılacak yöntem.

```csharp
public void OnFinish()
```

## Örnekler

Sayfa kaydetme geri aramasını kullanarak çok sayfalı belgeyi kullanıcı tarafından sağlanan akışlara nasıl kaydedeceğinizi gösterir.

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
        // her sayfa akışını işle
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

### Ayrıca Bakınız

* interface [IPageSavingCallback](../)
* namespace [Aspose.Tasks.Saving](../../ipagesavingcallback/)
* assembly [Aspose.Tasks](../../../)


