---
title: "WorkingTimeCollection.Add"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة WorkingTimeCollection. تضيف نسخة جديدة من WorkingTime إلى هذه المجموعة"
type: docs
weight: 30
url: /ar/net/aspose.tasks/workingtimecollection/add/
---
## WorkingTimeCollection.Add method

يضيف نسخة جديدة من WorkingTime إلى هذه المجموعة.

```csharp
public bool Add(WorkingTime item)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| العنصر | WorkingTime | العنصر المراد إضافته. |

### قيمة الإرجاع

صحيح إذا تم إضافة كائن WorkingTime بنجاح؛ وإلا، خطأ.

## الأمثلة

يوضح كيفية العمل مع مجموعة أوقات العمل.

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Custom Calendar");

calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));

var saturdayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(8, 12),
    new WorkingTime(13, 15)
};
var saturday = new WeekDay(DayType.Saturday);
foreach (var time in saturdayWorkingTimes)
{
    saturday.WorkingTimes.Add(time);
}

// اطبع أوقات العمل ليوم السبت
Console.WriteLine("Saturday working period number: " + saturday.WorkingTimes.Count);
foreach (var time in saturday.WorkingTimes)
{
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

var sundayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(10, 15)
};
var sunday = new WeekDay(DayType.Sunday, sundayWorkingTimes);

// اطبع أوقات العمل ليوم الأحد
List<WorkingTime> workingTimes = sunday.WorkingTimes.ToList();
Console.WriteLine("Sunday working period number: " + workingTimes.Count);
for (var index = 0; index < workingTimes.Count; index++)
{
    var time = workingTimes[index];
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

calendar.WeekDays.Add(saturday);
calendar.WeekDays.Add(sunday);

foreach (var day in calendar.WeekDays)
{
    Console.WriteLine(day.DayType + ": ");

    // يمكنك أيضًا التنقل عبر أوقات العمل وعرضها
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine(workingTime.From);
        Console.WriteLine(workingTime.To);
    }

    Console.WriteLine();
}
```

### انظر أيضًا

* class [WorkingTime](../../workingtime/)
* class [WorkingTimeCollection](../)
* namespace [Aspose.Tasks](../../workingtimecollection/)
* assembly [Aspose.Tasks](../../../)


