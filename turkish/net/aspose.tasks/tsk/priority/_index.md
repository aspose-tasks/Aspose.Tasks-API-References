---
title: "Tsk.Priority"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir göreve verilen önem seviyesidir; bu da kaynak dengelemesi sırasında bir görevin veya atamanın ne kadar kolay gecikebileceğini veya bölünebileceğini gösterir."
type: docs
weight: 930
url: /tr/net/aspose.tasks/tsk/priority/
---
## Tsk.Priority field

Bir göreve verilen önem seviyesi, bunun da kaynak dengelemesi sırasında bir görevin veya atamanın ne kadar kolay geciktirilebileceğini veya bölünebileceğini gösterir.

```csharp
public static readonly Key<int, TaskKey> Priority;
```

## Örnekler

Görev önceliğini okumanın nasıl yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "TaskPriority.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Tüm görevler için öncelikleri görüntüle.
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name) + " - Priority : " + task.Get(Tsk.Priority));
}
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


