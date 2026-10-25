---
title: "Класс MPPSaveOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Saving.MPPSaveOptions. Позволяет указать дополнительные параметры при сохранении данных проекта в MPP"
type: docs
weight: 2050
url: /ru/net/aspose.tasks.saving/mppsaveoptions/
---
## MPPSaveOptions class

Позволяет указать дополнительные параметры при сохранении данных проекта в MPP.

```csharp
public class MPPSaveOptions : SimpleSaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [MPPSaveOptions](mppsaveoptions/)() | Инициализирует новый экземпляр класса `MPPSaveOptions`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [ClearVba](../../aspose.tasks.saving/mppsaveoptions/clearvba/) { get; set; } | Получает или задает значение, указывающее, следует ли удалять существующие данные макросов VBA при сохранении проекта в формат MPP. |
| [ProtectionPassword](../../aspose.tasks.saving/mppsaveoptions/protectionpassword/) { get; set; } | Получает или задает пароль, используемый для защиты получаемого файла MPP. В настоящее время поддерживается для форматов MS Project 2010 и новее. Значение null указывает, что файл проекта не защищён. |
| [RemoveInvalidAssignments](../../aspose.tasks.saving/mppsaveoptions/removeinvalidassignments/) { get; set; } | Получает или задает значение, указывающее, следует ли удалять недействительные назначения ресурсов при сохранении в MPP. MS Project создает пустое назначение ресурса для каждой задачи. Установите этот флаг в true, чтобы удалять их при сохранении. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Получает или задает формат, в котором будет сохраняться документ, если используется этот объект параметров сохранения. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Получает или задает компаратор для сортировки задач на диаграмме Ганта и листе задач. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Получает или задает условие, используемое для фильтрации задач, отрисованных на диаграммах Ганта, листе задач и использовании задач. |
| [WriteFilters](../../aspose.tasks.saving/mppsaveoptions/writefilters/) { get; set; } | Получает или задает значение, указывающее, следует ли записывать данные фильтров при сохранении проекта в формат MPP. Данные фильтров включают коллекции Project.TaskFilters и Project.ResourceFilters. |
| [WriteGroups](../../aspose.tasks.saving/mppsaveoptions/writegroups/) { get; set; } | Получает или задает значение, указывающее, следует ли записывать данные групп при сохранении проекта в формат MPP. Данные групп включают коллекции Project.TaskGroups и Project.ResourceGroups. |
| [WriteVba](../../aspose.tasks.saving/mppsaveoptions/writevba/) { get; set; } | Получает или задает значение, указывающее, следует ли обновлять существующие данные макросов VBA в файле MPP. В настоящее время поддерживается запись VbaModule.SourceCode. |
| [WriteViewData](../../aspose.tasks.saving/mppsaveoptions/writeviewdata/) { get; set; } | Получает или задает значение, указывающее, следует ли записывать данные представлений при сохранении проекта в формат MPP. Данные представлений включают коллекции Project.Views, Filters и Tables. |

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

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


