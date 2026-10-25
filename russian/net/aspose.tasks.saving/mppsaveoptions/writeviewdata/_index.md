---
title: "MPPSaveOptions.WriteViewData"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство MPPSaveOptions. Возвращает или задает значение, указывающее, следует ли записывать данные представлений при сохранении проекта в формат MPP. Данные представлений включают коллекции Project.Views, Filters и Tables."
type: docs
weight: 80
url: /ru/net/aspose.tasks.saving/mppsaveoptions/writeviewdata/
---
## MPPSaveOptions.WriteViewData property

Получает или задает значение, указывающее, следует ли записывать данные представлений при сохранении проекта в формат MPP. Данные представлений включают коллекции Project.Views, Filters и Tables.

```csharp
public bool WriteViewData { get; set; }
```

## Примеры

Показывает, как сохранить проект в поток в виде файла MPP.

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

    // создать параметры сохранения
    SimpleSaveOptions options = new MPPSaveOptions
    {
        // задаёт значение, указывающее, следует ли удалять недействительные назначения ресурсов при сохранении в MPP
        RemoveInvalidAssignments = true
    };

    // сохранить MPP с параметрами
    project.Save(stream, options);
}
```

### См. также

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


