---
title: "Duration.Add"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Duration yöntemi. Belirtilen süreyi bu süreye ekler"
type: docs
weight: 60
url: /tr/net/aspose.tasks/duration/add/
---
## Add(Duration) {#add}

Bu süreye belirtilen süreyi ekler.

```csharp
public Duration Add(Duration d)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| d | Duration | Bu örneğe eklenecek belirtilen [`Duration`](../). |

### Dönüş Değeri

Bu örneğin değerini belirtilen süre değerine ekleyen yeni bir süre nesnesi.

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

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)

---

## Add(double) {#add_1}

Bu süreye belirtilen çift değer ekler.

```csharp
public Duration Add(double val)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| val | Double | Bu örneğe eklenecek belirtilen Double değeri. |

### Dönüş Değeri

Bu örneğin değerini belirtilen süre değerine ekleyen yeni bir süre nesnesi.

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

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


