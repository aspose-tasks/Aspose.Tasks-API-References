---
title: "Duration.Subtract"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Duration yöntemi. Belirtilen süreyi bu süre örneğinden çıkarır."
type: docs
weight: 100
url: /tr/net/aspose.tasks/duration/subtract/
---
## Subtract(Duration) {#subtract}

Bu süre örneğinden belirtilen süreyi çıkarır.

```csharp
public Duration Subtract(Duration d)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| d | Duration | Bu örnekten çıkarılacak belirtilen [`Duration`](../) örneği. |

### Dönüş Değeri

Bu örneğin değerini belirtilen süre değerinden çıkaran yeni süre nesnesi.

## Örnekler

Görevlerin süresini nasıl değiştireceğinizi gösterir.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// bir görev al
var task1 = project.RootTask.Children.GetById(1);

// görev süresini güncelle
var duration1 = task1.Get(Tsk.Duration);

// görev 1'den bir gün çıkar.
duration1 = duration1.Subtract(project.GetDuration(1, TimeUnitType.Day));

// göreve yeni bir süre ayarla
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// başka bir görev al
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// gerçek zaman birimi tipini kullanarak süreyi değiştir
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Subtract(1d /* the time unit type of duration2 will be used */);

// göreve yeni bir süre ayarla
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task2.Get(Tsk.Duration));
```

### Ayrıca Bakınız

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)

---

## Subtract(double) {#subtract_1}

Bu süre örneğinden belirtilen çift değeri çıkarır.

```csharp
public Duration Subtract(double val)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| val | Double | Bu örnekten çıkarılacak belirtilen Double değer. |

### Dönüş Değeri

Bu örneğin değerini belirtilen süre değerinden çıkaran yeni süre nesnesi.

## Örnekler

Görevlerin süresini nasıl değiştireceğinizi gösterir.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// bir görev al
var task1 = project.RootTask.Children.GetById(1);

// görev süresini güncelle
var duration1 = task1.Get(Tsk.Duration);

// görev 1'den bir gün çıkar.
duration1 = duration1.Subtract(project.GetDuration(1, TimeUnitType.Day));

// göreve yeni bir süre ayarla
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// başka bir görev al
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// gerçek zaman birimi tipini kullanarak süreyi değiştir
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Subtract(1d /* the time unit type of duration2 will be used */);

// göreve yeni bir süre ayarla
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task2.Get(Tsk.Duration));
```

### Ayrıca Bakınız

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


