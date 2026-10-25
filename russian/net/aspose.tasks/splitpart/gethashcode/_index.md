---
title: "SplitPart.GetHashCode"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод SplitPart. Возвращает значение хеш‑кода для экземпляра класса SplitPart."
type: docs
weight: 40
url: /ru/net/aspose.tasks/splitpart/gethashcode/
---
## SplitPart.GetHashCode method

Возвращает значение хеш‑кода для экземпляра класса [`SplitPart`](../).

```csharp
public override int GetHashCode()
```

### Возвращаемое значение

возвращает значение хеш‑кода для этого объекта.

## Примеры

Показывает, как получить хеш‑код части разбиения.

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

// равенство частей разбиения проверяется относительно начала, окончания и индекса частей разбиения.
var part1 = task.SplitParts[0];
var part2 = task.SplitParts[1];

// хеш‑код части разбиения, основанный на начале, окончании и индексе части разбиения.
Console.WriteLine("Split Part 1 Start {0} Finish {1} HashCode {2}", part1.Start, part1.Finish, part1.GetHashCode());
Console.WriteLine("Split Part 2 Start {0} Finish {1} HashCode {2}", part2.Start, part2.Finish, part2.GetHashCode());
```

### См. также

* class [SplitPart](../)
* namespace [Aspose.Tasks](../../splitpart/)
* assembly [Aspose.Tasks](../../../)


