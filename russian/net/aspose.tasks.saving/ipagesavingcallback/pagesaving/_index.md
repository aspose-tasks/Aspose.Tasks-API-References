---
title: "IPageSavingCallback.PageSaving"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод IPageSavingCallback. Метод, который будет вызван, когда страница сохраняется в поток."
type: docs
weight: 20
url: /ru/net/aspose.tasks.saving/ipagesavingcallback/pagesaving/
---
## IPageSavingCallback.PageSaving method

Метод, который будет вызван, когда страница сохраняется в поток.

```csharp
public void PageSaving(PageSavingArgs args)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| args | PageSavingArgs | Аргументы сохранения страницы. |

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

* class [PageSavingArgs](../../pagesavingargs/)
* interface [IPageSavingCallback](../)
* namespace [Aspose.Tasks.Saving](../../ipagesavingcallback/)
* assembly [Aspose.Tasks](../../../)


