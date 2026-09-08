---
title: "Класс TasksReadingException"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.TasksReadingException. Представляет стандартный внутренний тип исключения чтения"
type: docs
weight: 2540
url: /ru/net/aspose.tasks/tasksreadingexception/
---
## TasksReadingException class

Представляет стандартный внутренний тип исключения чтения.

```csharp
public class TasksReadingException : TasksLoggedException
```

## Свойства

| Имя | Описание |
| --- | --- |
| [LogText](../../aspose.tasks/tasksloggedexception/logtext/) { get; } | Получает информацию о журналировании исключения. |
| [Operation](../../aspose.tasks/tasksloggedexception/operation/) { get; } | Получает информацию об операции исключения. |

## Примеры

Показывает, как обрабатывать исключения чтения/записи проекта.

```csharp
try
{
    var project = new Project(DataDir + "project.mpp");
    project.Save(OutDir + "HandleExceptions_out.mpp", SaveFileFormat.Mpp);
}
catch (TasksReadingException ex)
{
    Console.WriteLine("Message: ");
    Console.WriteLine(ex.Message);
    Console.WriteLine("Log: ");
    Console.WriteLine(ex.LogText);
    if (ex.InnerException != null)
    {
        Console.WriteLine("Inner exception message: ");
        Console.WriteLine(ex.InnerException.Message);
    }
}
```

### См. также

* class [TasksLoggedException](../tasksloggedexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


