---
title: "TaskBaseline.EstimatedDuration"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TaskBaseline özelliği. Görevin baseline süresinin tahmini olup olmadığını gösteren bir değeri alır veya ayarlar"
type: docs
weight: 30
url: /tr/net/aspose.tasks/taskbaseline/estimatedduration/
---
## TaskBaseline.EstimatedDuration property

Görevin temel çizgi süresinin tahmini olup olmadığını gösteren bir değeri alır veya ayarlar.

```csharp
public bool EstimatedDuration { get; set; }
```

## Örnekler

Bir temel çizgi bilgisine nasıl erişileceğini gösterir.

```csharp
var project = new Project();

// TaskBaseline Oluşturma
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// Görev temel çizgi süresini göster
var baseline = task.Baselines.ToList()[0];
Console.WriteLine("Baseline Start: {0}", baseline.Start);
Console.WriteLine("Baseline duration: {0}", baseline.Duration);
Console.WriteLine("Baseline duration format: {0}", baseline.Duration.TimeUnit);
Console.WriteLine("Is it estimated duration?: {0}", baseline.EstimatedDuration);
Console.WriteLine("Baseline Finish: {0}", baseline.Finish);

// Bunun geçici bir temel çizgi olup olmadığını gösteren değer
Console.WriteLine("Interim: {0}", baseline.Interim);
Console.WriteLine("Fixed Cost: {0}", baseline.FixedCost);

// Görev temel çizgi zaman aşamalı verilerini yazdır
Console.WriteLine("Number of timephased items: " + baseline.TimephasedData.Count);
foreach (var data in baseline.TimephasedData)
{
    Console.WriteLine(" Uid: " + data.Uid);
    Console.WriteLine(" Start: " + data.Start);
    Console.WriteLine(" Finish: " + data.Finish);
}
```

### Ayrıca Bakınız

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


