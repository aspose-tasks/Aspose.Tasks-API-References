---
title: "الفئة WorkingTimeCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.WorkingTimeCollection. تمثل مجموعة من كائنات WorkingTimeCollection"
type: docs
weight: 3670
url: /ar/net/aspose.tasks/workingtimecollection/
---
## WorkingTimeCollection class

تمثل مجموعة من كائنات `WorkingTimeCollection`.

```csharp
public class WorkingTimeCollection : IList<WorkingTime>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/workingtimecollection/count/) { get; } | يحصل على عدد الكائنات المحتواة في كائن `WorkingTimeCollection` هذا. |
| [Item](../../aspose.tasks/workingtimecollection/item/) { get; set; } | يرجع العنصر عند الفهرس المحدد. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks/workingtimecollection/add/)(WorkingTime) | يضيف نسخة جديدة من WorkingTime إلى هذه المجموعة. |
| [Clear](../../aspose.tasks/workingtimecollection/clear/)() | يزيل جميع عناصر [`WorkingTime`](../workingtime/) من المجموعة. |
| [Contains](../../aspose.tasks/workingtimecollection/contains/)(WorkingTime) | يتحقق مما إذا كان العنصر المحدد موجودًا في القائمة. ينفذ بحثًا خطيًا O(n). |
| [CopyTo](../../aspose.tasks/workingtimecollection/copyto/)(WorkingTime[], int) | ينسخ محتوى مجموعة إلى Array، بدءًا من فهرس معين. |
| [GetEnumerator](../../aspose.tasks/workingtimecollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [Remove](../../aspose.tasks/workingtimecollection/remove/)(WorkingTime) | يزيل نسخة [`WorkingTime`](../workingtime/) من هذه المجموعة. |
| [ToList](../../aspose.tasks/workingtimecollection/tolist/)() | يحول كائن WorkingTimeCollection إلى قائمة من كائنات [`WorkingTime`](../workingtime/). |

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

* class [WorkingTime](../workingtime/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


