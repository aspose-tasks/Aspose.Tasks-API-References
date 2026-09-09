---
title: "Tsk.OutlineLevel"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin taslak seviyesi"
type: docs
weight: 840
url: /tr/net/aspose.tasks/tsk/outlinelevel/
---
## Tsk.OutlineLevel field

Bir görevin anahat seviyesi.

```csharp
public static readonly Key<int, TaskKey> OutlineLevel;
```

## Örnekler

Görev taslak özelliklerini nasıl okuyacağınızı gösterir.

```csharp
var project = new Project(DataDir + "TaskOutlineProperties.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Toplanan tüm görevleri ayrıştır
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name) + " - Outline Level : " + task.Get(Tsk.OutlineLevel));
    Console.WriteLine(task.Get(Tsk.Name) + " - Outline Number : " + task.Get(Tsk.OutlineNumber));
}
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


