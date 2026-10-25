---
title: "Tsk.Calendar"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Tsk field. Календарь задачи"
type: docs
weight: 160
url: /ru/net/aspose.tasks/tsk/calendar/
---
## Tsk.Calendar field

Календарь задачи.

```csharp
public static readonly Key<Calendar, TaskKey> Calendar;
```

## Примеры

Показывает, как читать/записывать календари задач.

```csharp
var project = new Project(DataDir + "ReadTaskCalendar.mpp");
var task = project.RootTask.Children.Add("Task1");

// Создать календарь и назначить задаче
var newCalendar = project.Calendars.Add("TaskCal1");
task.Set(Tsk.Calendar, newCalendar);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Разобрать всех рекурсивных дочерних элементов
foreach (var tsk in collector.Tasks)
{
    var calendar = tsk.Get(Tsk.Calendar);
    Console.WriteLine("Task calendar name: {0}", calendar == null ? "None" : calendar.Name);
}
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


