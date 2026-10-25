---
title: "SimpleSaveOptions.SaveFormat"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SimpleSaveOptions özelliği. Belgenin bu kaydetme seçenekleri nesnesi kullanıldığında kaydedileceği biçimi alır veya ayarlar"
type: docs
weight: 10
url: /tr/net/aspose.tasks.saving/simplesaveoptions/saveformat/
---
## SimpleSaveOptions.SaveFormat property

Bu kaydetme seçenekleri nesnesi kullanılırsa belgenin kaydedileceği biçimi alır veya ayarlar.

```csharp
public SaveFileFormat SaveFormat { get; }
```

## Örnekler

MS Project dosyası kaydedilirken özel görev filtresi nasıl kullanılır gösterir.

```csharp
public void WorkWithTasksFilter()
{
    var project = new Project(DataDir + "CreateProject2.mpp");

    var options = new PdfSaveOptions
    {
        PresentationFormat = PresentationFormat.GanttChart,
        PageSize = PageSize.A3,
        StartDate = new DateTime(2010, 7, 1),
        EndDate = new DateTime(2010, 9, 1),

        // Görev 'Task5' ve 'Task3' atlanacak şekilde bir görev filtresi ayarla
        TasksFilter = new CustomTasksFilter()
    };

    // kaydetme formatını kontrol edelim
    Console.WriteLine("The save format: " + options.SaveFormat);

    // ...

    // projeyi bir görüntü olarak kaydet
    project.Save(OutDir + "WorkWithTasksFilter_out.png", options);
}

/// <summary>
/// MS Project dosyası (örneğin) PDF formatında kaydedilirken kullanılabilecek özel görev filtresi örneği.
/// </summary>
/// <inheritdoc />
private class CustomTasksFilter : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.Name) != "Task5" && el.Get(Tsk.Name) != "Task3";
    }
}
```

### Ayrıca Bakınız

* enum [SaveFileFormat](../../savefileformat/)
* class [SimpleSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../simplesaveoptions/)
* assembly [Aspose.Tasks](../../../)


