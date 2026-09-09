---
title: "Enum DayType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.DayType enum'ı. Haftanın gününü belirtir"
type: docs
weight: 450
url: /tr/net/aspose.tasks/daytype/
---
## DayType enumeration

Bir haftanın gününü belirtir.

```csharp
public enum DayType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Exception | `0` | İstisna gün tipini gösterir. |
| Sunday | `1` | Pazar gün tipini gösterir. |
| Monday | `2` | Pazartesi gün tipini gösterir. |
| Tuesday | `3` | Salı gün tipini gösterir. |
| Wednesday | `4` | Çarşamba gün tipini gösterir. |
| Thursday | `5` | Perşembe gün tipini gösterir. |
| Friday | `6` | Cuma gün tipini gösterir. |
| Saturday | `7` | Cumartesi gün tipini gösterir. |

## Örnekler

Yeni bir takvim nasıl tanımlanır, haftanın günleri nasıl eklenir ve günler için çalışma zamanları nasıl belirlenir gösterir.

```csharp
var project = new Project();

// Bir takvim tanımla
var calendar = project.Calendars.Add("Calendar1");

// Pazartesiden perşembeye varsayılan zamanlarla çalışma günleri ekle
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Cuma gününü kısa çalışma günü olarak ayarla
var weekDay = new WeekDay(DayType.Friday);

// Çalışma zamanını ayarlar. Yalnızca DateTime'ın zaman kısmı önemlidir.
var workingTime = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 16);
weekDay.WorkingTimes.Add(workingTime);
weekDay.WorkingTimes.Add(workingTime2);
weekDay.DayWorking = true;
calendar.WeekDays.Add(weekDay);

// projeyle çalışılıyor...
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


