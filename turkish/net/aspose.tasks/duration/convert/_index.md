---
title: "Duration.Convert"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Duration yöntemi. Duration nesnesini belirtilen zaman birimleriyle başka bir süreye dönüştürür"
type: docs
weight: 70
url: /tr/net/aspose.tasks/duration/convert/
---
## Duration.Convert method

Duration nesnesini belirtilen zaman birimleriyle başka bir süreye dönüştürür.

```csharp
public Duration Convert(TimeUnitType timeUnitType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| timeUnitType | TimeUnitType | belirtilen zaman birimi türü. |

### Dönüş Değeri

belirtilen birim türüyle yeni bir süre döndürür.

## Örnekler

Bir sürenin farklı zaman birimi türlerine nasıl dönüştürüleceğini gösterir.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// Görevi, süresini farklı biçimlerde hesaplaması için alın
var task = project.RootTask.Children.GetById(1);

// Dakika, Gün, Saat, Hafta ve Ay cinsinden süreyi alın
var mins = task.Get(Tsk.Duration).Convert(TimeUnitType.Minute).ToDouble();
Console.WriteLine("Duration in Mins: {0}", mins);
var days = task.Get(Tsk.Duration).Convert(TimeUnitType.Day).ToDouble();
Console.WriteLine("Duration in Days: {0}", days);
var hours = task.Get(Tsk.Duration).Convert(TimeUnitType.Hour).ToDouble();
Console.WriteLine("Duration in Hours: {0}", hours);
var weeks = task.Get(Tsk.Duration).Convert(TimeUnitType.Week).ToDouble();
Console.WriteLine("Duration in Weeks: {0}", weeks);
var months = task.Get(Tsk.Duration).Convert(TimeUnitType.Month).ToDouble();
Console.WriteLine("Duration in Months: {0}", months);
```

### Ayrıca Bakınız

* enum [TimeUnitType](../../timeunittype/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


