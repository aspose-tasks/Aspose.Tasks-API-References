---
title: "Interface IPageSavingCallback"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Saving.IPageSavingCallback interface. Представляет обратный вызов, который вызывается при сохранении каждой страницы многостраничного документа в отдельный поток."
type: docs
weight: 2020
url: /ru/net/aspose.tasks.saving/ipagesavingcallback/
---
## IPageSavingCallback interface

Представляет обратный вызов, который вызывается, когда каждая страница в многостраничном документе сохраняется в отдельный поток.

```csharp
public interface IPageSavingCallback
```

## Методы

| Имя | Описание |
| --- | --- |
| [OnFinish](../../aspose.tasks.saving/ipagesavingcallback/onfinish/)() | Метод, который будет вызван после записи всех страниц. |
| [PageSaving](../../aspose.tasks.saving/ipagesavingcallback/pagesaving/)(PageSavingArgs) | Метод, который будет вызван, когда страница сохраняется в поток. |

## Примеры

Показывает, как сохранить многостраничный документ в пользовательские потоки, используя обратный вызов сохранения страниц.

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
        // обрабатывать каждый поток страницы
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

### См. также

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


