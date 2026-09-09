---
title: "Arayüz IPageSavingCallback"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Saving.IPageSavingCallback arayüzü. Çok sayfalı belgede her sayfa ayrı bir akıma kaydedildiğinde çağrılan bir geri aramayı temsil eder"
type: docs
weight: 2020
url: /tr/net/aspose.tasks.saving/ipagesavingcallback/
---
## IPageSavingCallback interface

Çok sayfalı belgede her sayfa ayrı bir akışa kaydedildiğinde çağrılan bir geri aramayı temsil eder.

```csharp
public interface IPageSavingCallback
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [OnFinish](../../aspose.tasks.saving/ipagesavingcallback/onfinish/)() | Tüm sayfalar yazıldığında çağrılacak yöntem. |
| [PageSaving](../../aspose.tasks.saving/ipagesavingcallback/pagesaving/)(PageSavingArgs) | Bir sayfa bir akışa kaydedildiğinde çağrılacak yöntem. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


