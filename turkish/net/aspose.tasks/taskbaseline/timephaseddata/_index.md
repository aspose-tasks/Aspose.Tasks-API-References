---
title: "TaskBaseline.TimephasedData"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TaskBaseline özelliği. Bu nesne için bir TimephasedDataCollection örneğini alır veya ayarlar. Görev baseline'ı ile ilişkili zaman aşamalı veri."
type: docs
weight: 80
url: /tr/net/aspose.tasks/taskbaseline/timephaseddata/
---
## TaskBaseline.TimephasedData property

Bu nesne için bir TimephasedDataCollection örneğini alır veya ayarlar. Görev temel çizgisiyle ilişkili zaman aşamalı veriler.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
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

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


