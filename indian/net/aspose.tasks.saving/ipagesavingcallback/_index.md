---
title: "इंटरफ़ेस IPageSavingCallback"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Saving.IPageSavingCallback interface. एक कॉलबैक को दर्शाता है जो प्रत्येक पेज को मल्टी पेज दस्तावेज़ में अलग स्ट्रीम में सहेजे जाने पर कॉल किया जाता है"
type: docs
weight: 2020
url: /hi/net/aspose.tasks.saving/ipagesavingcallback/
---
## IPageSavingCallback interface

एक कॉलबैक को दर्शाता है जो मल्टी पेज दस्तावेज़ में प्रत्येक पेज को अलग स्ट्रीम में सहेजते समय कॉल किया जाता है।

```csharp
public interface IPageSavingCallback
```

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [OnFinish](../../aspose.tasks.saving/ipagesavingcallback/onfinish/)() | वह मेथड जो सभी पेज लिखे जाने पर कॉल किया जाएगा। |
| [PageSaving](../../aspose.tasks.saving/ipagesavingcallback/pagesaving/)(PageSavingArgs) | पेज को स्ट्रीम में सहेजा जाने पर कॉल की जाने वाली विधि। |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


