---
title: "Tsk.Duration"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Общий промежуток активного рабочего времени задачи, введённый или рассчитанный Microsoft Project на основе даты начала, даты завершения, календарей и других факторов планирования"
type: docs
weight: 300
url: /ru/net/aspose.tasks/tsk/duration/
---
## Tsk.Duration field

Общий промежуток активного рабочего времени задачи, введённый или рассчитанный Microsoft Project на основе даты начала, даты завершения, календарей и других факторов планирования.

```csharp
public static readonly Key<Duration, TaskKey> Duration;
```

## Примеры

Показывает, как установить длительность задачи.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Start, new DateTime(2012, 8, 23, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.ActualStart, new DateTime(2012, 8, 23, 8, 0, 0));

project.Save(OutDir + "AddTaskDuration_out.xml", SaveFileFormat.Xml);
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


