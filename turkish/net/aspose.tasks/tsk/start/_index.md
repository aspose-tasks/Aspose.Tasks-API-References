---
title: "Tsk.Start"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin planlanan başlangıç tarihi"
type: docs
weight: 1010
url: /tr/net/aspose.tasks/tsk/start/
---
## Tsk.Start field

Bir görevin planlanan başlangıç tarihi.

```csharp
public static readonly Key<DateTime, TaskKey> Start;
```

## Örnekler

Görev özelliklerini okuma/yazma yöntemini gösterir.

```csharp
var project = new Project();

// Görev ekle ve görev özelliklerini ayarla
var task = project.RootTask.Children.Add();
task.Set(Tsk.Name, "Task1");
task.Set(Tsk.Start, new DateTime(2020, 3, 31, 8, 0, 0));
task.Set(Tsk.Finish, new DateTime(2020, 3, 31, 17, 0, 0));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Toplanan tüm görevleri ayrıştır
foreach (var tsk in collector.Tasks)
{
    Console.WriteLine("Task Id: {0}", tsk.Get(Tsk.Id));
    Console.WriteLine("Task Uid: {0}", tsk.Get(Tsk.Uid));
    Console.WriteLine("Task Name: {0}", tsk.Get(Tsk.Name));
    Console.WriteLine("Task Start: {0}", tsk.Get(Tsk.Start));
    Console.WriteLine("Task Finish: {0}", tsk.Get(Tsk.Finish));
}
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


