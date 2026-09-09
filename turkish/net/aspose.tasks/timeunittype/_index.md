---
title: "Enum TimeUnitType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.TimeUnitType enum. Bir zaman biriminin tipini belirtir"
type: docs
weight: 2570
url: /tr/net/aspose.tasks/timeunittype/
---
## TimeUnitType enumeration

Bir zaman biriminin türünü belirtir.

```csharp
public enum TimeUnitType : sbyte
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Undefined | `-1` | Tanımsız değerin, alanın orijinal proje dosyasında tanımlanmadığını gösterir. |
| Minute | `0` | Dakika zaman birimi tipini belirtir. |
| ElapsedMinute | `1` | Geçen dakika zaman birimi tipini belirtir. |
| Hour | `2` | Saat zaman birimi tipini belirtir. |
| ElapsedHour | `3` | Geçen saat zaman birimi tipini belirtir. |
| Day | `4` | Gün zaman birimi tipini belirtir. |
| ElapsedDay | `5` | Geçen gün zaman birimi tipini belirtir. |
| Week | `6` | Hafta zaman birimi tipini belirtir. |
| ElapsedWeek | `7` | Geçen hafta zaman birimi tipini belirtir. |
| Month | `8` | Ay zaman birimi tipini belirtir. |
| ElapsedMonth | `9` | Geçen ay zaman birimi tipini belirtir. |
| Percent | `10` | Yüzde zaman birimi tipini belirtir. |
| ElapsedPercent | `11` | Geçen yüzde zaman birimi tipini belirtir. |
| Null | `12` | Boş zaman birimi tipini belirtir. |
| MinuteEstimated | `13` | Dakika tahmini zaman birimi tipini belirtir. |
| ElapsedMinuteEstimated | `14` | Geçen dakika tahmini zaman birimi tipini belirtir. |
| HourEstimated | `15` | Saat tahmini zaman birimi tipini belirtir. |
| ElapsedHourEstimated | `16` | Geçen saat tahmini zaman birimi tipini belirtir. |
| DayEstimated | `17` | Gün tahmini zaman birimi tipini belirtir. |
| ElapsedDayEstimated | `18` | Geçen gün tahmini zaman birimi tipini belirtir. |
| WeekEstimated | `19` | Hafta tahmini zaman birimi tipini belirtir. |
| ElapsedWeekEstimated | `20` | Geçen hafta tahmini zaman birimi tipini belirtir. |
| MonthEstimated | `21` | Ay tahmini zaman birimi tipini belirtir. |
| ElapsedMonthEstimated | `22` | Geçen ay tahmini zaman birimi tipini belirtir. |
| PercentEstimated | `23` | Yüzde tahmini zaman birimi tipini belirtir. |
| ElapsedPercentEstimated | `24` | Geçen yüzde tahmini zaman birimi türünü belirtir. |
| Year | `25` | Yıl zaman birimi türünü belirtir. |

## Açıklamalar

XML'e dışa aktarırken Tanımsız değerler sonuç XML'inden kaldırılacaktır.

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


