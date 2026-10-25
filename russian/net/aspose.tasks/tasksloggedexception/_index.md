---
title: "Класс TasksLoggedException"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.TasksLoggedException. Представляет стандартный внутренний тип исключения"
type: docs
weight: 2530
url: /ru/net/aspose.tasks/tasksloggedexception/
---
## TasksLoggedException class

Представляет стандартный внутренний тип исключения.

```csharp
public class TasksLoggedException : ApplicationException
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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


