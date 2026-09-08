---
title: "Класс TaskValidationException"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.TaskValidationException. Представляет исключение, которое выбрасывается, когда после пересчёта обнаруживаются ошибки в задачах проекта."
type: docs
weight: 2510
url: /ru/net/aspose.tasks/taskvalidationexception/
---
## TaskValidationException class

Представляет исключение, которое выбрасывается, когда после перерасчёта обнаруживаются ошибки в задачах проекта.

```csharp
public class TaskValidationException : RecalculationValidationException
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Task](../../aspose.tasks/taskvalidationexception/task/) { get; } | Получает задачу, вызвавшую исключение. |

## Примеры

Показывает, при каких условиях исключение &lt;see cref=\"TaskValidationException\" /&gt; может быть выброшено.

```csharp
try
{
    var project = new Project { CalculationMode = CalculationMode.None };
    var task = project.RootTask.Children.Add("Task");

    // неумышленно задать неверные даты
    task.Set(Tsk.Start, new DateTime(2017, 6, 19, 8, 0, 0));
    task.Set(Tsk.Duration, project.GetDuration(1));
    task.Set(Tsk.Finish, new DateTime(2017, 6, 18, 17, 0, 0));

    // выполнить пересчёт проекта с флагом для запуска проверки
    project.Recalculate(true);
}
catch (TaskValidationException ex)
{
    Console.WriteLine(ex.Message);
}
```

### См. также

* class [RecalculationValidationException](../recalculationvalidationexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


