---
title: "Duration.TimeUnit"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Duration özelliği. Bu nesne için zaman birimi tipini alır. Bu Duration örneğinin zaman birimi tipi."
type: docs
weight: 50
url: /tr/net/aspose.tasks/duration/timeunit/
---
## Duration.TimeUnit property

Bu nesne için zaman birimi türünü alır. Bu Duration örneğinin zaman birimi türü.

```csharp
public TimeUnitType TimeUnit { get; }
```

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

* enum [TimeUnitType](../../timeunittype/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


