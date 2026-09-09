---
title: "Tsk.WBSLevel"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin en sağdaki WBS seviyesi"
type: docs
weight: 1140
url: /tr/net/aspose.tasks/tsk/wbslevel/
---
## Tsk.WBSLevel field

Bir görevin en sağdaki WBS seviyesi.

```csharp
public static readonly Key<string, TaskKey> WBSLevel;
```

## Örnekler

Görevin WBS kodlarını nasıl okuyacağınızı gösterir.

```csharp
var project = new Project(DataDir + "TaskWBS.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Toplanan tüm görevleri ayrıştır
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.WBS));
    Console.WriteLine(task.Get(Tsk.WBSLevel));
}
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


