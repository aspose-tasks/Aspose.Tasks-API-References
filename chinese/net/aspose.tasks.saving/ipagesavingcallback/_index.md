---
title: "接口 IPageSavingCallback"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Saving.IPageSavingCallback 接口。表示在多页文档的每一页保存到单独流时被调用的回调"
type: docs
weight: 2020
url: /zh/net/aspose.tasks.saving/ipagesavingcallback/
---
## IPageSavingCallback interface

表示在将多页文档的每一页保存到单独的流时调用的回调。

```csharp
public interface IPageSavingCallback
```

## 方法

| 名称 | 描述 |
| --- | --- |
| [OnFinish](../../aspose.tasks.saving/ipagesavingcallback/onfinish/)() | 当所有页面写入完成后将被调用的方法。 |
| [PageSaving](../../aspose.tasks.saving/ipagesavingcallback/pagesaving/)(PageSavingArgs) | 当页面保存到流时要调用的方法。 |

## 示例

展示如何使用页面保存回调将多页文档保存到用户提供的流中。

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
        // 处理每个页面流
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

### 另见

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


