---
title: "IPageSavingCallback.PageSaving"
second_title: "Aspose.Tasks for .NET API 참조"
description: "IPageSavingCallback 메서드. 페이지가 스트림에 저장될 때 호출되는 메서드"
type: docs
weight: 20
url: /ko/net/aspose.tasks.saving/ipagesavingcallback/pagesaving/
---
## IPageSavingCallback.PageSaving method

페이지가 스트림에 저장될 때 호출되는 메서드.

```csharp
public void PageSaving(PageSavingArgs args)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| args | PageSavingArgs | 페이지 저장 인수입니다. |

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

* class [PageSavingArgs](../../pagesavingargs/)
* interface [IPageSavingCallback](../)
* namespace [Aspose.Tasks.Saving](../../ipagesavingcallback/)
* assembly [Aspose.Tasks](../../../)


