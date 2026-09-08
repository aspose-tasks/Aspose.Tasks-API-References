---
title: "TasksLoggedException.Operation"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство TasksLoggedException. Возвращает информацию о операции исключения"
type: docs
weight: 20
url: /ru/net/aspose.tasks/tasksloggedexception/operation/
---
## TasksLoggedException.Operation property

Получает информацию об операции исключения.

```csharp
public string Operation { get; }
```

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

* class [TasksLoggedException](../)
* namespace [Aspose.Tasks](../../tasksloggedexception/)
* assembly [Aspose.Tasks](../../../)


