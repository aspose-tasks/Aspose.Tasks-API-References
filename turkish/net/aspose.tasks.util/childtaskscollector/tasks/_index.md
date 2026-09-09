---
title: "ChildTasksCollector.Tasks"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ChildTasksCollector özelliği. Toplanan alt nesne görevlerinin bir listesini alır"
type: docs
weight: 20
url: /tr/net/aspose.tasks.util/childtaskscollector/tasks/
---
## ChildTasksCollector.Tasks property

Toplanan alt nesnelerin (görevlerin) bir listesini alır.

```csharp
public List<Task> Tasks { get; }
```

## Örnekler

Bir projedeki tüm görevler üzerinde düz bir liste olarak nasıl yineleme yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Toplanan tüm görevleri ayrıştır
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### Ayrıca Bakınız

* class [Task](../../../aspose.tasks/task/)
* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


