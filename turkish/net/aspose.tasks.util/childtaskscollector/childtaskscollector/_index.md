---
title: "ChildTasksCollector.ChildTasksCollector"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ChildTasksCollector yapıcı. ChildTasksCollector sınıfının yeni bir örneğini başlatır"
type: docs
weight: 10
url: /tr/net/aspose.tasks.util/childtaskscollector/childtaskscollector/
---
## ChildTasksCollector constructor

[`ChildTasksCollector`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public ChildTasksCollector()
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

* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


