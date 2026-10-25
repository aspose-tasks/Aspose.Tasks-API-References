---
title: "DailyCalendarRepetition.DailyCalendarRepetition"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "DailyCalendarRepetition constructor. DailyCalendarRepetition क्लास का नया इंस्टेंस प्रारंभ करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks/dailycalendarrepetition/dailycalendarrepetition/
---
## DailyCalendarRepetition constructor

[`DailyCalendarRepetition`](../) क्लास का नया इंस्टेंस प्रारंभ करता है।

```csharp
public DailyCalendarRepetition()
```

## उदाहरण

दैनिक कार्य पुनरावृत्ति पैटर्न की पुनरावृत्तियों और '24 घंटे' के साथ आवर्ती कार्य बनाने के दौरान कैसे काम करें, यह दर्शाता है।

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

// परियोजना के साथ आगे काम करें...
project.Save(OutDir + "CanAddRecurringTask_Days_CalendarDays_24h_Test_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* class [DailyCalendarRepetition](../)
* namespace [Aspose.Tasks](../../dailycalendarrepetition/)
* assembly [Aspose.Tasks](../../../)


