---
title: "Tsk.Calendar"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Görev takvimi"
type: docs
weight: 160
url: /tr/net/aspose.tasks/tsk/calendar/
---
## Tsk.Calendar field

Görev takvimi.

```csharp
public static readonly Key<Calendar, TaskKey> Calendar;
```

## Örnekler

Görev takvimlerini okuma/yazma yöntemini gösterir.

```csharp
var project = new Project(DataDir + "ReadTaskCalendar.mpp");
var task = project.RootTask.Children.Add("Task1");

// Takvim oluştur ve göreve ata
var newCalendar = project.Calendars.Add("TaskCal1");
task.Set(Tsk.Calendar, newCalendar);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Tüm yinelemeli alt öğeleri ayrıştır
foreach (var tsk in collector.Tasks)
{
    var calendar = tsk.Get(Tsk.Calendar);
    Console.WriteLine("Task calendar name: {0}", calendar == null ? "None" : calendar.Name);
}
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


