---
title: IPageSavingCallback.PageSaving
second_title: Aspose.Tasks for .NET API Reference
description: IPageSavingCallback method. The method to be called when a page is saved to a stream
type: docs
weight: 20
url: /net/aspose.tasks.saving/ipagesavingcallback/pagesaving/
---
## IPageSavingCallback.PageSaving method

The method to be called when a page is saved to a stream.

```csharp
public void PageSaving(PageSavingArgs args)
```

| Parameter | Type | Description |
| --- | --- | --- |
| args | PageSavingArgs | The page saving arguments. |

## Examples

Shows how to save multi page document to user-provided streams using page saving callback.

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
        // process each page stream
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

### See Also

* class [PageSavingArgs](../../pagesavingargs/)
* interface [IPageSavingCallback](../)
* namespace [Aspose.Tasks.Saving](../../ipagesavingcallback/)
* assembly [Aspose.Tasks](../../../)


