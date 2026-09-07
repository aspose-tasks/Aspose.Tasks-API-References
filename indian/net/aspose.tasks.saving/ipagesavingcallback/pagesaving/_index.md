---
title: "IPageSavingCallback.PageSaving"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "IPageSavingCallback मेथड। वह मेथड जो किसी पृष्ठ को स्ट्रीम में सहेजे जाने पर कॉल किया जाएगा।"
type: docs
weight: 20
url: /hi/net/aspose.tasks.saving/ipagesavingcallback/pagesaving/
---
## IPageSavingCallback.PageSaving method

पेज को स्ट्रीम में सहेजा जाने पर कॉल की जाने वाली विधि।

```csharp
public void PageSaving(PageSavingArgs args)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| args | PageSavingArgs | पृष्ठ सहेजने के तर्क। |

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

* class [PageSavingArgs](../../pagesavingargs/)
* interface [IPageSavingCallback](../)
* namespace [Aspose.Tasks.Saving](../../ipagesavingcallback/)
* assembly [Aspose.Tasks](../../../)


