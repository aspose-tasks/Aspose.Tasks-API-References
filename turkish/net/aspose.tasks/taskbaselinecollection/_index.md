---
title: "Sınıf TaskBaselineCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.TaskBaselineCollection sınıfı. TaskBaseline nesnelerinin bir koleksiyonunu temsil eder."
type: docs
weight: 2380
url: /tr/net/aspose.tasks/taskbaselinecollection/
---
## TaskBaselineCollection class

[`TaskBaseline`](../taskbaseline/) nesnelerinin bir koleksiyonunu temsil eder.

```csharp
public class TaskBaselineCollection : IList<TaskBaseline>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks/taskbaselinecollection/count/) { get; } | Bu TaskBaselineCollection nesnesinde bulunan nesne sayısını alır. |
| [Item](../../aspose.tasks/taskbaselinecollection/item/) { get; set; } | Belirtilen indeksteki öğeyi döndürür. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks/taskbaselinecollection/add/)(TaskBaseline) | Bu, ICollection'ın Add metodunun sadece NotSupportedException fırlatan taslak uygulamasıdır |
| [GetEnumerator](../../aspose.tasks/taskbaselinecollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |
| [Remove](../../aspose.tasks/taskbaselinecollection/remove/)(TaskBaseline) | Bu koleksiyondan temel çizgiyi kaldırır. |
| [ToList](../../aspose.tasks/taskbaselinecollection/tolist/)() | TaskBaselineCollection nesnesini [`TaskBaseline`](../taskbaseline/) nesnelerinin bir listesine dönüştürür. |

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

* class [TaskBaseline](../taskbaseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


