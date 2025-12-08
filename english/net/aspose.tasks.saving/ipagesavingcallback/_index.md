---
title: Interface IPageSavingCallback
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Saving.IPageSavingCallback interface. Represents a callback that is called when each page in multi page document is saved to a separate stream
type: docs
weight: 1990
url: /net/aspose.tasks.saving/ipagesavingcallback/
---
## IPageSavingCallback interface

Represents a callback that is called when each page in multi page document is saved to a separate stream.

```csharp
public interface IPageSavingCallback
```

## Methods

| Name | Description |
| --- | --- |
| [OnFinish](../../aspose.tasks.saving/ipagesavingcallback/onfinish/)() | Method which will be called when all pages are written. |
| [PageSaving](../../aspose.tasks.saving/ipagesavingcallback/pagesaving/)(PageSavingArgs) | The method to be called when a page is saved to a stream. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


