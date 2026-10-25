---
title: "TaskBaselineCollection.ToList"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TaskBaselineCollection metodu. TaskBaselineCollection nesnesini TaskBaseline nesnelerinin bir listesine dönüştürür"
type: docs
weight: 60
url: /tr/net/aspose.tasks/taskbaselinecollection/tolist/
---
## TaskBaselineCollection.ToList method

TaskBaselineCollection nesnesini [`TaskBaseline`](../../taskbaseline/) nesnelerinin bir listesine dönüştürür.

```csharp
public List<TaskBaseline> ToList()
```

### Dönüş Değeri

Listesi [`TaskBaseline`](../../taskbaseline/) nesneleri.

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


