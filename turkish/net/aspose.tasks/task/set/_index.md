---
title: "Task.Set"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Task yöntemi. Belirtilen özelliği bu kapsayıcıda belirtilen değere eşler"
type: docs
weight: 1410
url: /tr/net/aspose.tasks/task/set/
---
## Task.Set&lt;T&gt; method

Belirtilen özelliği bu kapsayıcıda belirtilen değere eşler.

```csharp
public void Set<T>(Key<T, TaskKey> key, T val)
```

| Parametre | Açıklama |
| --- | --- |
| T | eşlenen değerin tipi. |
| key | belirtilen özellik anahtarı. [`Tsk`](../../tsk/) özellik anahtarını almak için. |
| val | değer. |

## Örnekler

Görev özelliklerini almayı/ayarlamayı gösterir.

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
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


