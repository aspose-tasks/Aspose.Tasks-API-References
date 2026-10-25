---
title: "DailyCalendarRepetition.DailyCalendarRepetition"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "DailyCalendarRepetition yapıcı. DailyCalendarRepetition sınıfının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/net/aspose.tasks/dailycalendarrepetition/dailycalendarrepetition/
---
## DailyCalendarRepetition constructor

[`DailyCalendarRepetition`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public DailyCalendarRepetition()
```

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

* class [DailyCalendarRepetition](../)
* namespace [Aspose.Tasks](../../dailycalendarrepetition/)
* assembly [Aspose.Tasks](../../../)


