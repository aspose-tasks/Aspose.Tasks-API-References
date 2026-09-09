---
title: "Sınıf TaskBaseline"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.TaskBaseline sınıfı. Bir görevin temel çizgisini temsil eder."
type: docs
weight: 2370
url: /tr/net/aspose.tasks/taskbaseline/
---
## TaskBaseline class

Bir Görevin Temel Çizgisini temsil eder.

```csharp
public sealed class TaskBaseline : Baseline, IComparable<TaskBaseline>, IEquatable<TaskBaseline>
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [TaskBaseline](taskbaseline/)(Task) | `TaskBaseline` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | Bir temel veri kaydının benzersiz numarasını alır veya ayarlar. |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | Bir kaynağın bir proje için şu ana kadar gerçekleştirdiği işin bütçelenen maliyetini alır veya ayarlar. |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | Bir kaynak için planlanan işin bütçe maliyetini alır veya ayarlar. |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | Temel kaydedildiğinde bir kaynağın öngörülen maliyetini alır veya ayarlar. |
| [Duration](../../aspose.tasks/taskbaseline/duration/) { get; set; } | Temel çizgi kaydedildiğinde görevin planlanan süresini alır veya ayarlar. |
| [EstimatedDuration](../../aspose.tasks/taskbaseline/estimatedduration/) { get; set; } | Görevin temel çizgi süresinin tahmini olup olmadığını gösteren bir değeri alır veya ayarlar. |
| [Finish](../../aspose.tasks/taskbaseline/finish/) { get; set; } | Temel çizgi kaydedildiğinde görevin planlanan bitiş tarihini alır veya ayarlar. |
| [FixedCost](../../aspose.tasks/taskbaseline/fixedcost/) { get; set; } | Temel çizgi kaydedildiğinde görevin sabit maliyetini alır veya ayarlar. |
| [Interim](../../aspose.tasks/taskbaseline/interim/) { get; set; } | Bunun geçici bir temel çizgi olup olmadığını gösteren bir değeri alır veya ayarlar. |
| [Start](../../aspose.tasks/taskbaseline/start/) { get; set; } | Temel çizgi kaydedildiğinde görevin planlanan başlangıç tarihini alır veya ayarlar. |
| [TimephasedData](../../aspose.tasks/taskbaseline/timephaseddata/) { get; set; } | Bu nesne için bir TimephasedDataCollection örneğini alır veya ayarlar. Görev temel çizgisiyle ilişkili zaman aşamalı veriler. |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | Temel kaydedildiğinde bir kaynağa atanan işi alır veya ayarlar. Temel kaydedildiğinde bir kaynağa atanan iş miktarıdır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | IComparable arabirimi uygulaması. Bu örneği belirtilen Baseline nesnesiyle karşılaştırır. |
| [CompareTo](../../aspose.tasks/taskbaseline/compareto/#compareto_1)(TaskBaseline) | IComparable arabirimi uygulaması. Bu örneği belirtilen Baseline nesnesiyle karşılaştırır. |
| [Equals](../../aspose.tasks/baseline/equals/)(Baseline) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| override [Equals](../../aspose.tasks/taskbaseline/equals/#equals_2)(object) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| [Equals](../../aspose.tasks/taskbaseline/equals/#equals_1)(TaskBaseline) | Bu örneğin belirtilen TaskBaseline nesnesine eşit olup olmadığını gösteren bir değer döndürür. |
| override [GetHashCode](../../aspose.tasks/taskbaseline/gethashcode/)() | `TaskBaseline` sınıfının örneği için bir karma kod değeri döndürür. |

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

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


