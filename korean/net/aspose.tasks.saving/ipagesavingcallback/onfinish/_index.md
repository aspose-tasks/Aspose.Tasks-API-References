---
title: "IPageSavingCallback.OnFinish"
second_title: "Aspose.Tasks for .NET API 참조"
description: "IPageSavingCallback 메서드. 모든 페이지가 기록될 때 호출되는 메서드"
type: docs
weight: 10
url: /ko/net/aspose.tasks.saving/ipagesavingcallback/onfinish/
---
## IPageSavingCallback.OnFinish method

모든 페이지가 기록될 때 호출되는 메서드.

```csharp
public void OnFinish()
```

## 예제

페이지 저장 콜백을 사용하여 사용자 제공 스트림에 다중 페이지 문서를 저장하는 방법을 보여줍니다.

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
        // 각 페이지 스트림을 처리합니다
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

### 또 보기

* interface [IPageSavingCallback](../)
* namespace [Aspose.Tasks.Saving](../../ipagesavingcallback/)
* assembly [Aspose.Tasks](../../../)


