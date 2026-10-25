---
title: "Класс TaskLink"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.TaskLink. Представляет предшествующую связь"
type: docs
weight: 2410
url: /ru/net/aspose.tasks/tasklink/
---
## TaskLink class

Представляет предшествующую связь.

```csharp
public sealed class TaskLink : IEquatable<TaskLink>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [CrossProjectName](../../aspose.tasks/tasklink/crossprojectname/) { get; set; } | Получает или задает внешний предшествующий проект. |
| [IsCrossProject](../../aspose.tasks/tasklink/iscrossproject/) { get; set; } | Получает или задает значение, указывающее, является ли предшественник частью другого проекта. |
| [LagFormat](../../aspose.tasks/tasklink/lagformat/) { get; set; } | Получает или задает формат представления задержки. |
| [LinkLag](../../aspose.tasks/tasklink/linklag/) { get; set; } | Получает или задает задержку в десятых долях минуты или в процентах. |
| [LinkLagTimeSpan](../../aspose.tasks/tasklink/linklagtimespan/) { get; set; } | Получает или задает длительность задержки в зависимости от LagFormat. |
| [LinkType](../../aspose.tasks/tasklink/linktype/) { get; set; } | Получает или задает тип ссылки. |
| [PredTask](../../aspose.tasks/tasklink/predtask/) { get; set; } | Получает или задает предшествующую задачу. |
| [SuccTask](../../aspose.tasks/tasklink/succtask/) { get; set; } | Получает или задает последующую задачу. |

## Методы

| Имя | Описание |
| --- | --- |
| override [Equals](../../aspose.tasks/tasklink/equals/#equals_1)(object) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту. |
| [Equals](../../aspose.tasks/tasklink/equals/#equals)(TaskLink) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту. |
| override [GetHashCode](../../aspose.tasks/tasklink/gethashcode/)() | Возвращает значение хеш-кода для экземпляра класса `TaskLink`. |
| override [ToString](../../aspose.tasks/tasklink/tostring/)() | Возвращает строковое представление TaskLink. Точные детали представления не указаны и могут измениться. |

## Примеры

Показывает, как читать ссылки задач проекта.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

// Отобразить имена предшествующей и последующей задач.
foreach (var taskLink in project.TaskLinks)
{
    Console.WriteLine("Predecessor: " + taskLink.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor: " + taskLink.SuccTask.Get(Tsk.Name));
    Console.WriteLine("Lag Format: " + taskLink.LagFormat);
    Console.WriteLine("Link Lag: " + taskLink.LinkLag);
    Console.WriteLine();
}
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


