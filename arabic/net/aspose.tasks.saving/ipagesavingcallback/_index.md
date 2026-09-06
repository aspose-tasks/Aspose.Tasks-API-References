---
title: "واجهة IPageSavingCallback"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Aspose.Tasks.Saving.IPageSavingCallback واجهة. تمثل رد نداء يتم استدعاؤه عندما يتم حفظ كل صفحة في مستند متعدد الصفحات إلى تدفق منفصل"
type: docs
weight: 2020
url: /ar/net/aspose.tasks.saving/ipagesavingcallback/
---
## IPageSavingCallback interface

يمثل رد نداء يتم استدعاؤه عندما يتم حفظ كل صفحة في مستند متعدد الصفحات إلى تدفق منفصل.

```csharp
public interface IPageSavingCallback
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| [OnFinish](../../aspose.tasks.saving/ipagesavingcallback/onfinish/)() | الطريقة التي سيتم استدعاؤها عندما تُكتب جميع الصفحات. |
| [PageSaving](../../aspose.tasks.saving/ipagesavingcallback/pagesaving/)(PageSavingArgs) | الطريقة التي يجب استدعاؤها عندما يتم حفظ صفحة إلى تدفق. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


