---
title: "Sınıf DailyCalendarRepetition"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.DailyCalendarRepetition sınıfı. Takvim günlerine dayalı günlük yinelenme desenindeki tekrarlar için bir sınıfı temsil eder"
type: docs
weight: 390
url: /tr/net/aspose.tasks/dailycalendarrepetition/
---
## DailyCalendarRepetition class

Takvim günlerine dayalı günlük yineleme desenindeki tekrarlar için bir sınıfı temsil eder.

```csharp
public class DailyCalendarRepetition : DailyRepetitionBase
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [DailyCalendarRepetition](dailycalendarrepetition/)() | `DailyCalendarRepetition` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/dailyrepetitionbase/repetitioninterval/) { get; set; } | Oluşumlar arasındaki gün cinsinden aralığı temsil eden gün sayısını alır veya ayarlar. |

## Örnekler

Yinelenen görevler oluştururken günlük iş tekrar deseni tekrarlarını ve '24 Saat' kavramını nasıl kullanacağınızı gösterir.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var calendar = project.Calendars.Add("24 Hours");
Calendar.Make24HourCalendar(calendar);
var parameters = new RecurringTaskParameters
{
    TaskName = "t1",
    Duration = project.GetDuration(1, TimeUnitType.Day),
    RecurrencePattern = new DailyRecurrencePattern
    {
        Repetition = new DailyCalendarRepetition { RepetitionInterval = 1 },
        RecurrenceRange = new EndByRecurrenceRange
        {
            Start = new DateTime(2018, 7, 2, 0, 0, 0),
            Finish = new DateTime(2018, 7, 8, 16, 0, 0)
        }
    }
};
parameters.SetCalendar(project, "24 Hours");
project.RootTask.Children.Add(parameters);

// projeyle daha fazla çalış...
project.Save(OutDir + "CanAddRecurringTask_Days_CalendarDays_24h_Test_out.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* class [DailyRepetitionBase](../dailyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


