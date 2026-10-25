---
title: "TaskBaselineCollection.Remove"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TaskBaselineCollection metodu. Bu koleksiyondan temel çizgiyi kaldırır"
type: docs
weight: 50
url: /tr/net/aspose.tasks/taskbaselinecollection/remove/
---
## TaskBaselineCollection.Remove method

Bu koleksiyondan temel çizgiyi kaldırır.

```csharp
public bool Remove(TaskBaseline item)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| öğe | TaskBaseline | Kaldırılacak öğe. |

### Dönüş Değeri

Öğe başarıyla kaldırıldıysa true; aksi takdirde false

## Örnekler

Görev temel çizgi koleksiyonlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project();

// proje temel çizgileri oluştur
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// görev temel çizgilerini yazdır
Console.WriteLine("Count of task baselines: " + task.Baselines.Count);
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration: {0}", baseline.Duration);
    Console.WriteLine("Baseline start: {0}", baseline.Start);
    Console.WriteLine("Baseline finish: {0}", baseline.Finish);
}

// tüm temel çizgileri temizleyelim
List<TaskBaseline> baselines = task.Baselines.ToList();
for (var i = 0; i < baselines.Count; i++)
{
    task.Baselines.Remove(baselines[i]);
}
```

### Ayrıca Bakınız

* class [TaskBaseline](../../taskbaseline/)
* class [TaskBaselineCollection](../)
* namespace [Aspose.Tasks](../../taskbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


