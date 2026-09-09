---
title: "TaskBaselineCollection.Count"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TaskBaselineCollection özelliği. Bu TaskBaselineCollection nesnesinde bulunan nesne sayısını alır."
type: docs
weight: 10
url: /tr/net/aspose.tasks/taskbaselinecollection/count/
---
## TaskBaselineCollection.Count property

Bu TaskBaselineCollection nesnesinde bulunan nesne sayısını alır.

```csharp
public int Count { get; }
```

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

* class [TaskBaselineCollection](../)
* namespace [Aspose.Tasks](../../taskbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


