---
title: "Класс TasksWritingException"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.TasksWritingException. Представляет стандартный внутренний тип исключения записи"
type: docs
weight: 2560
url: /ru/net/aspose.tasks/taskswritingexception/
---
## TasksWritingException class

Представляет стандартный внутренний тип исключения записи.

```csharp
public class TasksWritingException : TasksLoggedException
```

## Свойства

| Имя | Описание |
| --- | --- |
| [LogText](../../aspose.tasks/tasksloggedexception/logtext/) { get; } | Получает информацию о журналировании исключения. |
| [Operation](../../aspose.tasks/tasksloggedexception/operation/) { get; } | Получает информацию об операции исключения. |

## Примеры

Показывает, как читать текст журнала и тип исключения для проверки проблем с экспортом MPP.

```csharp
try
{
    var project = new Project(DataDir + "PrintTaskWritingException.mpp");

    // Экспортировать проект в файл MPP
    project.Save(OutDir + "PrintTaskWritingException_out.MPP", SaveFileFormat.Mpp);
}
catch (TasksWritingException ex)
{
    Console.WriteLine("Exception Operation: " + ex.Operation);
    Console.WriteLine("Exception Log Text: ");
    Console.WriteLine(ex.LogText);
}
```

### См. также

* class [TasksLoggedException](../tasksloggedexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


