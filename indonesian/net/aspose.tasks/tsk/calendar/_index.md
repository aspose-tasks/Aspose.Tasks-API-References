---
title: "Tsk.Calendar"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Tsk field. Kalender tugas"
type: docs
weight: 160
url: /id/net/aspose.tasks/tsk/calendar/
---
## Tsk.Calendar field

Kalender tugas.

```csharp
public static readonly Key<Calendar, TaskKey> Calendar;
```

## Contoh

Menampilkan cara membaca/menulis kalender tugas.

```csharp
var project = new Project(DataDir + "ReadTaskCalendar.mpp");
var task = project.RootTask.Children.Add("Task1");

// Buat kalender dan tetapkan ke tugas
var newCalendar = project.Calendars.Add("TaskCal1");
task.Set(Tsk.Calendar, newCalendar);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Mengurai semua anak secara rekursif
foreach (var tsk in collector.Tasks)
{
    var calendar = tsk.Get(Tsk.Calendar);
    Console.WriteLine("Task calendar name: {0}", calendar == null ? "None" : calendar.Name);
}
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


