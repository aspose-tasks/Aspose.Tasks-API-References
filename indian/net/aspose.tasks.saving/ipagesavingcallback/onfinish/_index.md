---
title: "IPageSavingCallback.OnFinish"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "IPageSavingCallback मेथड। वह मेथड जो सभी पृष्ठ लिखे जाने पर कॉल किया जाएगा।"
type: docs
weight: 10
url: /hi/net/aspose.tasks.saving/ipagesavingcallback/onfinish/
---
## IPageSavingCallback.OnFinish method

वह मेथड जो सभी पेज लिखे जाने पर कॉल किया जाएगा।

```csharp
public void OnFinish()
```

## उदाहरण

पेज सहेजने के कॉलबैक का उपयोग करके उपयोगकर्ता-प्रदान किए गए स्ट्रीम में मल्टी पेज दस्तावेज़ को कैसे सहेजें, यह दर्शाता है।

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
        // प्रत्येक पेज स्ट्रीम को प्रोसेस करें
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

### संबंधित देखें

* interface [IPageSavingCallback](../)
* namespace [Aspose.Tasks.Saving](../../ipagesavingcallback/)
* assembly [Aspose.Tasks](../../../)


