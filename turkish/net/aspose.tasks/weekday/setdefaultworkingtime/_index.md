---
title: "WeekDay.SetDefaultWorkingTime"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "WeekDay yöntemi. Belirtilen hafta günü için varsayılan zaman dilimlerini ayarlar"
type: docs
weight: 130
url: /tr/net/aspose.tasks/weekday/setdefaultworkingtime/
---
## WeekDay.SetDefaultWorkingTime method

Belirtilen hafta günü için varsayılan zaman dilimlerini ayarlar.

```csharp
public static void SetDefaultWorkingTime(WeekDay day)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| gün | WeekDay | Varsayılan çalışma gününün ayarlanacağı hafta günü. |

## Örnekler

Bir gün için varsayılan çalışma zamanının nasıl ayarlanacağını gösterir.

```csharp
var project = new Project();

// Bir takvim tanımla
var calendar = project.Calendars.Add("Calendar1");
calendar.WeekDays.Clear();

// Pazartesiden perşembeye varsayılan zamanlarla çalışma günleri ekle
var monday = new WeekDay(DayType.Monday);
WeekDay.SetDefaultWorkingTime(monday);
calendar.WeekDays.Add(monday);
var tuesday = new WeekDay(DayType.Tuesday);
WeekDay.SetDefaultWorkingTime(tuesday);
calendar.WeekDays.Add(tuesday);
var wednesday = new WeekDay(DayType.Wednesday);
WeekDay.SetDefaultWorkingTime(wednesday);
calendar.WeekDays.Add(wednesday);
var thursday = new WeekDay(DayType.Thursday);
WeekDay.SetDefaultWorkingTime(thursday);
calendar.WeekDays.Add(thursday);
var friday = new WeekDay(DayType.Friday);
WeekDay.SetDefaultWorkingTime(friday);
calendar.WeekDays.Add(friday);

var saturday = new WeekDay(DayType.Saturday);
saturday.DayWorking = false;
calendar.WeekDays.Add(saturday);
var sunday = new WeekDay(DayType.Sunday);
sunday.DayWorking = false;
calendar.WeekDays.Add(sunday);

// tüm çalışma zamanlarını yazdıralım
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine("Day Type: " + day.DayType); 
    Console.WriteLine("Is working day: " + day.DayWorking); 
    Console.WriteLine("Working Time (Hours): " + day.GetWorkingTime().TotalHours);
    Console.WriteLine();
}
```

### Ayrıca Bakınız

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


