---
title: "Класс SplitPart"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.SplitPart. Представляет часть задачи. SplitPart является элементом коллекции SplitParts задач."
type: docs
weight: 2290
url: /ru/net/aspose.tasks/splitpart/
---
## SplitPart class

Представляет часть задачи. SplitPart является элементом коллекции SplitParts задачи.

```csharp
public class SplitPart
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Finish](../../aspose.tasks/splitpart/finish/) { get; } | Получает дату завершения SplitPart. |
| [Start](../../aspose.tasks/splitpart/start/) { get; } | Получает дату начала SplitPart. |

## Методы

| Имя | Описание |
| --- | --- |
| override [Equals](../../aspose.tasks/splitpart/equals/)(object) | Сравнивает два SplitPart. |
| override [GetHashCode](../../aspose.tasks/splitpart/gethashcode/)() | Возвращает значение хеш‑кода для экземпляра класса `SplitPart`. |

## Примеры

Показывает, как работать с частями разделённой задачи.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 3, 21, 17, 0, 0));

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.IsManual, false);
task.Set(Tsk.Start, new DateTime(2000, 3, 15, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(3));

var assignment = project.ResourceAssignments.Add(task, project.Resources.Add("r1"));
assignment.Set(Asn.Start, new DateTime(2000, 3, 15, 8, 0, 0));
assignment.Set(Asn.Work, task.Get(Tsk.Work));
assignment.Set(Asn.Finish, new DateTime(2000, 3, 19, 17, 0, 0));

// необходимо сначала сгенерировать временные данные назначения ресурсов
assignment.TimephasedDataFromTaskDuration(project.Get(Prj.Calendar));

// разделить задачу.
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 17, 17, 0, 0), project.Get(Prj.Calendar));

// итерация по частям задачи
Console.WriteLine("Number of split parts: " + task.SplitParts.Count);
foreach (var splitPart in task.SplitParts)
{
    Console.WriteLine("  Split Part Start: " + splitPart.Start);
    Console.WriteLine("  Split Part Finish: " + splitPart.Finish);
    Console.WriteLine();
}
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


