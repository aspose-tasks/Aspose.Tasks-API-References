---
title: "ChildTasksCollector.Alg"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ChildTasksCollector yöntemi. Belirtilen nesneyi işler"
type: docs
weight: 30
url: /tr/net/aspose.tasks.util/childtaskscollector/alg/
---
## ChildTasksCollector.Alg method

Belirtilen nesneyi işler.

```csharp
public override void Alg(Task el, int level)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| el | Görev | İşlenecek nesne. |
| seviye | Int32 | Ağaç düğüm seviyesi. |

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


