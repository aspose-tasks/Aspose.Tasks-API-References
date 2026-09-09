---
title: "Sınıf TaskUtils"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Util.TaskUtils sınıfı. Görevlerle ilgili faydalı işlemler sağlayan yardımcı sınıf"
type: docs
weight: 2770
url: /tr/net/aspose.tasks.util/taskutils/
---
## TaskUtils class

Görevlerle ilgili kullanışlı işlemler sağlayan yardımcı sınıf.

```csharp
public static class TaskUtils
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [Apply](../../aspose.tasks.util/taskutils/apply/)(Task, ITreeAlgorithm&lt;Task&gt;, int) | Belirtilen algoritmayı bir ağacın her görevine uygular. |
| static [Filter](../../aspose.tasks.util/taskutils/filter/)(Task, ICondition&lt;Task&gt;) | Koşulu sağlayan görevlerden yeni bir ağaç oluşturur. |
| static [Find](../../aspose.tasks.util/taskutils/find/)(Task, ICondition&lt;Task&gt;) | Görev ağacında koşulu sağlayan bir görevi bulur. |
| static [TaskChildrenCount](../../aspose.tasks.util/taskutils/taskchildrencount/)(Task) | Tüm seviyelerde görevlerin alt görev sayısını özyinelemeli olarak hesaplar. |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


