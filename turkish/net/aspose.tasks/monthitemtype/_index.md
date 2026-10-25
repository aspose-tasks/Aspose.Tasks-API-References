---
title: "MonthItemType enum"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.MonthItemType enum. Bir istisna yinelemesinin planlandığı ay öğesini belirtir."
type: docs
weight: 1050
url: /tr/net/aspose.tasks/monthitemtype/
---
## MonthItemType enumeration

İstisna tekrarı planlanan ay öğesini belirtir.

```csharp
public enum MonthItemType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Undefined | `-1` | Tanımsız ay öğesi türünü gösterir. |
| Day | `0` | Gün ay öğesi türünü gösterir. |
| Weekday | `1` | Hafta içi ay öğesi türünü gösterir. |
| WeekendDay | `2` | Hafta sonu günü ay öğesi türünü gösterir. |
| Sunday | `3` | Pazar ay öğesi türünü gösterir. |
| Monday | `4` | Pazartesi ay öğesi türünü gösterir. |
| Tuesday | `5` | Salı ay öğesi türünü gösterir. |
| Wednesday | `6` | Çarşamba ay öğesi türünü gösterir. |
| Thursday | `7` | Perşembe ay öğesi türünü gösterir. |
| Friday | `8` | Cuma ay öğesi türünü gösterir. |
| Saturday | `9` | Cumartesi ay öğesi türünü gösterir. |

## Örnekler

Ay günüyle takvim istisnasının nasıl tanımlanacağını gösterir.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// takvim oluştur
var calendar = project.Calendars.Add("Calendar1");

// her cuma için takvim istisnası oluştur
var exception = new CalendarException();
exception.Type = CalendarExceptionType.MonthlyByDay;
exception.FromDate = new DateTime(2010, 1, 1);
exception.ToDate = new DateTime(2020, 12, 31);
exception.Month = Month.December;
exception.MonthDay = 1;
exception.MonthItem = MonthItemType.Undefined;
exception.MonthPosition = MonthPosition.Last;
exception.Period = 5;

// bir cuma gününün istisnai olduğunu kontrol et
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2012, 12, 1)));

// istisnayı takvime ekle
calendar.Exceptions.Add(exception);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


