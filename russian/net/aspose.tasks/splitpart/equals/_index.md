---
title: "SplitPart.Equals"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод SplitPart. Сравнивает две разделённые части"
type: docs
weight: 30
url: /ru/net/aspose.tasks/splitpart/equals/
---
## SplitPart.Equals method

Сравнивает два SplitPart.

```csharp
public override bool Equals(object obj)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | Объект | Объект для сравнения. |

### Возвращаемое значение

True, если указанный объект равен текущему объекту; в противном случае — false.

## Примеры

Показывает, как проверить равенство частей разбиения.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 3, 21, 17, 0, 0));

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.IsManual, false);
task.Set(Tsk.Start, new DateTime(2000, 3, 15, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(4));

var assignment = project.ResourceAssignments.Add(task, project.Resources.Add("Resource"));
assignment.Set(Asn.Start, new DateTime(2000, 3, 15, 8, 0, 0));
assignment.Set(Asn.Work, task.Get(Tsk.Work));
assignment.Set(Asn.Finish, new DateTime(2000, 3, 19, 17, 0, 0));

// необходимо сначала сгенерировать временные данные назначения ресурсов
assignment.TimephasedDataFromTaskDuration(project.Get(Prj.Calendar));
Console.WriteLine(assignment.Get(Asn.Finish));

// разделить задачу.
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 17, 17, 0, 0), project.Get(Prj.Calendar));

// равенство частей разбиения проверяется относительно начала, окончания и индекса частей разбиения.
var part1 = task.SplitParts[0];
var part2 = task.SplitParts[1];
Console.WriteLine("Split Part 1 Start {0} Finish {1}", part1.Start, part1.Finish);
Console.WriteLine("Split Part 2 Start {0} Finish {1}", part2.Start, part2.Finish);
Console.WriteLine("Are split parts equal: " + part1.Equals(part2));
```

### См. также

* class [SplitPart](../)
* namespace [Aspose.Tasks](../../splitpart/)
* assembly [Aspose.Tasks](../../../)


