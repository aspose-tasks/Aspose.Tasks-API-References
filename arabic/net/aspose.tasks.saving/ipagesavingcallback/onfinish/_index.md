---
title: "IPageSavingCallback.OnFinish"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة IPageSavingCallback. الطريقة التي سيتم استدعاؤها عندما يتم كتابة جميع الصفحات"
type: docs
weight: 10
url: /ar/net/aspose.tasks.saving/ipagesavingcallback/onfinish/
---
## IPageSavingCallback.OnFinish method

الطريقة التي سيتم استدعاؤها عندما تُكتب جميع الصفحات.

```csharp
public void OnFinish()
```

## الأمثلة

يوضح كيفية حفظ مستند متعدد الصفحات إلى تدفقات يقدمها المستخدم باستخدام رد نداء حفظ الصفحة.

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
        // معالجة تدفق كل صفحة
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

### انظر أيضًا

* interface [IPageSavingCallback](../)
* namespace [Aspose.Tasks.Saving](../../ipagesavingcallback/)
* assembly [Aspose.Tasks](../../../)


