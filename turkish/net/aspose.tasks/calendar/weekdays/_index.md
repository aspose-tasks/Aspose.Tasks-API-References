---
title: "Calendar.WeekDays"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Calendar özelliği. Bu takvim için WeekDaysCollection nesnesini alır. Takvimi tanımlayan hafta içi günlerinin koleksiyonu."
type: docs
weight: 120
url: /tr/net/aspose.tasks/calendar/weekdays/
---
## Calendar.WeekDays property

Bu takvim için WeekDaysCollection'ı alır. Takvimi tanımlayan hafta içi günlerinin koleksiyonunu içerir.

```csharp
public WeekDayCollection WeekDays { get; }
```

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

* class [WeekDayCollection](../../weekdaycollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


