---
title: "Yapı Duration"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Duration yapısı. Bir projedeki süreyi temsil eder"
type: docs
weight: 470
url: /tr/net/aspose.tasks/duration/
---
## Duration structure

Bir projedeki süreyi temsil eder.

```csharp
public struct Duration : IEquatable<Duration>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [IsElapsed](../../aspose.tasks/duration/iselapsed/) { get; } | Zaman biriminin geçmiş olup olmadığını gösteren bir değer alır. Bu Duration örneğinin geçmiş olup olmadığını belirleyen bayrak. |
| [IsEstimated](../../aspose.tasks/duration/isestimated/) { get; } | Zaman biriminin tahmini olup olmadığını gösteren bir değer alır. Bu Duration örneğinin tahmini olup olmadığını belirleyen bayrak. |
| [TimeSpan](../../aspose.tasks/duration/timespan/) { get; } | Bu Duration nesnesinin [`TimeSpan`](./timespan/) örneğini alır. Bu Duration nesnesinin TimeSpan örneği. |
| [TimeUnit](../../aspose.tasks/duration/timeunit/) { get; } | Bu nesne için zaman birimi türünü alır. Bu Duration örneğinin zaman birimi türü. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [Parse](../../aspose.tasks/duration/parse/)(Project, string) | Belirtilen dizeyi `Duration` yapısının örneğine dönüştürür. |
| [Add](../../aspose.tasks/duration/add/#add_1)(double) | Bu süreye belirtilen çift değer ekler. |
| [Add](../../aspose.tasks/duration/add/#add)(Duration) | Bu süreye belirtilen süreyi ekler. |
| [Convert](../../aspose.tasks/duration/convert/)(TimeUnitType) | Duration nesnesini belirtilen zaman birimleriyle başka bir süreye dönüştürür. |
| [Equals](../../aspose.tasks/duration/equals/#equals)(Duration) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| override [Equals](../../aspose.tasks/duration/equals/#equals_1)(object) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| override [GetHashCode](../../aspose.tasks/duration/gethashcode/)() | Bu nesne için bir karma kod değeri döndürür. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract_1)(double) | Bu süre örneğinden belirtilen çift değeri çıkarır. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract)(Duration) | Bu süre örneğinden belirtilen süreyi çıkarır. |
| [ToDouble](../../aspose.tasks/duration/todouble/)() | Duration nesnesini Double değere dönüştürür. |
| override [ToString](../../aspose.tasks/duration/tostring/)() | Bu örneğin dize temsili döndürür. |
| static [ParseTimeSpan](../../aspose.tasks/duration/parsetimespan/)(string) | \"PT--H--M--S--\" biçimindeki süre dizesini ayrıştırır. |
| [operator ==](../../aspose.tasks/duration/op_equality/) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| [operator !=](../../aspose.tasks/duration/op_inequality/) | Bu örneğin belirtilen nesneye eşit olmadığını gösteren bir değer döndürür. |

## Örnekler

Görevlerin süresini nasıl güncelleyeceğinizi gösterir.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// bir görev al
var task1 = project.RootTask.Children.GetById(1);

// görev süresini güncelle
var duration1 = task1.Get(Tsk.Duration);

// görev 1'e bir gün ekle
duration1 = duration1.Add(project.GetDuration(1, TimeUnitType.Day));

// göreve yeni bir süre ayarla
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// başka bir görev al
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// gerçek zaman birimi tipini kullanarak süreyi değiştir
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Add(1d /* the time unit type of duration2 will be used */);

// göreve yeni bir süre ayarla
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task1.Get(Tsk.Duration));
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


