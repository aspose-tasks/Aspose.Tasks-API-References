---
title: "TasksFilter"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Получает или задает условие, используемое для фильтрации задач, отображаемых на листе задач Ганта и диаграммах использования задач."
type: docs
weight: 190
url: /ru/net/aspose.tasks.saving/saveoptions/tasksfilter/
---
## SaveOptions.TasksFilter property

Получает или задает условие, используемое для фильтрации задач, отрисованных на диаграммах Ганта, листе задач и использовании задач.

```csharp
public ICondition<Task> TasksFilter { get; set; }
```

### Примечания

Если значение не указано, используется фильтр по умолчанию, который удаляет невидимые задачи — то есть дочерние задачи свернутых задач.

### Примеры

Показывает, как использовать пользовательский фильтр задач при сохранении файла MS Project.

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

        // Установите фильтр задач, чтобы пропустить задачи 'Task5' и 'Task3'.
        TasksFilter = new CustomTasksFilter()
    };

    // Давайте проверим формат сохранения
    Console.WriteLine("The save format: " + options.SaveFormat);

    // ...

    // сохранить проект как изображение
    project.Save(OutDir + "WorkWithTasksFilter_out.png", options);
}

/// <summary>
/// Пример пользовательского фильтра задач, который можно использовать при сохранении файла MS Project (например) в формате PDF.
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

### См. также

* interface [ICondition&lt;T&gt;](../../../aspose.tasks.util/icondition-1)
* class [Task](../../../aspose.tasks/task)
* class [SaveOptions](../../saveoptions)
* namespace [Aspose.Tasks.Saving](../../saveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для Aspose.Tasks.dll -->
