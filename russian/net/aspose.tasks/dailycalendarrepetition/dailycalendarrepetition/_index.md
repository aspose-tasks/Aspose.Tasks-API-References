---
title: "DailyCalendarRepetition.DailyCalendarRepetition"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор DailyCalendarRepetition. Инициализирует новый экземпляр класса DailyCalendarRepetition"
type: docs
weight: 10
url: /ru/net/aspose.tasks/dailycalendarrepetition/dailycalendarrepetition/
---
## DailyCalendarRepetition constructor

Инициализирует новый экземпляр класса [`DailyCalendarRepetition`](../).

```csharp
public DailyCalendarRepetition()
```

## Примеры

Показывает, как работать с повторениями шаблона ежедневных задач и '24 Hours' при создании повторяющихся задач.

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

// работайте с проектом дальше...
project.Save(OutDir + "CanAddRecurringTask_Days_CalendarDays_24h_Test_out.mpp", SaveFileFormat.Mpp);
```

### См. также

* class [DailyCalendarRepetition](../)
* namespace [Aspose.Tasks](../../dailycalendarrepetition/)
* assembly [Aspose.Tasks](../../../)


