---
title: "TaskUtils.Apply"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TaskUtils yöntemi. Belirtilen algoritmayı bir ağacın her görevine uygular."
type: docs
weight: 10
url: /tr/net/aspose.tasks.util/taskutils/apply/
---
## TaskUtils.Apply method

Belirtilen algoritmayı bir ağacın her görevine uygular.

```csharp
public static void Apply(Task root, ITreeAlgorithm<Task> alg, int level)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| root | Görev | Ağacın kökü |
| alg | ITreeAlgorithm`1 | Uygulanan algoritma. |
| seviye | Int32 | Kök görevin seviyesi. |

## Örnekler

Ağaç algoritmasıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// tüm proje görevlerini topla
var coll = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, coll, 0);

// görevleri düz bir liste gibi işle
foreach (var task in coll.Tasks)
{
    Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
}
```

### Ayrıca Bakınız

* class [Task](../../../aspose.tasks/task/)
* interface [ITreeAlgorithm&lt;T&gt;](../../itreealgorithm-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


