---
title: "Класс TasksException"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.TasksException. Представляет стандартный внутренний тип исключения"
type: docs
weight: 2520
url: /ru/net/aspose.tasks/tasksexception/
---
## TasksException class

Представляет стандартный внутренний тип исключения.

```csharp
public class TasksException : ApplicationException
```

## Примеры

Показывает, как обнаружить повреждённую структуру проекта.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

// проверьте структуру проекта.
// Будет выброшено <see cref=\"TasksException\">, если структура проекта некорректна.
try
{
    TaskUtils.Apply(project.RootTask, new CheckCircuit(), 0);
}
catch (TasksException ex)
{
    Console.WriteLine(ex);
}
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


