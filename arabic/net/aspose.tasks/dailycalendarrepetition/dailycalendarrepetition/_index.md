---
title: "DailyCalendarRepetition.DailyCalendarRepetition"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ DailyCalendarRepetition. يهيئ مثيلًا جديدًا من فئة DailyCalendarRepetition"
type: docs
weight: 10
url: /ar/net/aspose.tasks/dailycalendarrepetition/dailycalendarrepetition/
---
## DailyCalendarRepetition constructor

يهيئ مثيلًا جديدًا من الفئة [`DailyCalendarRepetition`](../).

```csharp
public DailyCalendarRepetition()
```

## الأمثلة

يوضح كيفية العمل مع تكرارات نمط تكرار العمل اليومي و'24 ساعة' أثناء إنشاء مهام متكررة.

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

// العمل مع المشروع أكثر...
project.Save(OutDir + "CanAddRecurringTask_Days_CalendarDays_24h_Test_out.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* class [DailyCalendarRepetition](../)
* namespace [Aspose.Tasks](../../dailycalendarrepetition/)
* assembly [Aspose.Tasks](../../../)


