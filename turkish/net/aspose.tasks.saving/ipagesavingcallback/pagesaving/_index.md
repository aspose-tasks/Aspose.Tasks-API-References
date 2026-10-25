---
title: "IPageSavingCallback.PageSaving"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "IPageSavingCallback yöntemi. Bir sayfa bir akışa kaydedildiğinde çağrılacak yöntem"
type: docs
weight: 20
url: /tr/net/aspose.tasks.saving/ipagesavingcallback/pagesaving/
---
## IPageSavingCallback.PageSaving method

Bir sayfa bir akışa kaydedildiğinde çağrılacak yöntem.

```csharp
public void PageSaving(PageSavingArgs args)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| args | PageSavingArgs | Sayfa kaydetme argümanları. |

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

* class [PageSavingArgs](../../pagesavingargs/)
* interface [IPageSavingCallback](../)
* namespace [Aspose.Tasks.Saving](../../ipagesavingcallback/)
* assembly [Aspose.Tasks](../../../)


