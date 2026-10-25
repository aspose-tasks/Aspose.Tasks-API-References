---
title: "Класс DailyCalendarRepetition"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.DailyCalendarRepetition. Представляет класс для повторений в ежедневном шаблоне повторения, основанном на календарных днях"
type: docs
weight: 390
url: /ru/net/aspose.tasks/dailycalendarrepetition/
---
## DailyCalendarRepetition class

Представляет класс для повторений в ежедневном шаблоне повторения, основанном на календарных днях.

```csharp
public class DailyCalendarRepetition : DailyRepetitionBase
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [DailyCalendarRepetition](dailycalendarrepetition/)() | Инициализирует новый экземпляр класса `DailyCalendarRepetition`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/dailyrepetitionbase/repetitioninterval/) { get; set; } | Получает или задает количество дней, которое представляет интервал в днях между вхождениями. |

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

* class [DailyRepetitionBase](../dailyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


