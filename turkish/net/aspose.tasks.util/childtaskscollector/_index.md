---
title: "Sınıf ChildTasksCollector"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Util.ChildTasksCollector sınıfı. Tüm alt görevleri toplar"
type: docs
weight: 2690
url: /tr/net/aspose.tasks.util/childtaskscollector/
---
## ChildTasksCollector class

Tüm alt görevleri toplar.

```csharp
public class ChildTasksCollector : TreeAlgorithmBase<Task>
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ChildTasksCollector](childtaskscollector/)() | `ChildTasksCollector` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Tasks](../../aspose.tasks.util/childtaskscollector/tasks/) { get; } | Toplanan alt nesnelerin (görevlerin) bir listesini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [Alg](../../aspose.tasks.util/childtaskscollector/alg/)(Task, int) | Belirtilen nesneyi işler. |
| virtual [PostAlg](../../aspose.tasks.util/treealgorithmbase-1/postalg/)(Task, int) |  |
| virtual [PreAlg](../../aspose.tasks.util/treealgorithmbase-1/prealg/)(Task, int) |  |

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

* class [TreeAlgorithmBase&lt;T&gt;](../treealgorithmbase-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


