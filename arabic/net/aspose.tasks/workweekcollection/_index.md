---
title: "الفئة WorkWeekCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.WorkWeekCollection. تمثل مجموعة من كائنات WorkWeek"
type: docs
weight: 3650
url: /ar/net/aspose.tasks/workweekcollection/
---
## WorkWeekCollection class

تمثل مجموعة من كائنات [`WorkWeek`](../workweek/).

```csharp
public class WorkWeekCollection : IList<WorkWeek>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/workweekcollection/count/) { get; } | يحصل على عدد الكائنات المحتواة في كائن `WorkWeekCollection` هذا. |
| [Item](../../aspose.tasks/workweekcollection/item/) { get; set; } | يرجع العنصر عند الفهرس المحدد. |
| [ParentCalendar](../../aspose.tasks/workweekcollection/parentcalendar/) { get; } | يحصل على التقويم الأب. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks/workweekcollection/add/)(WorkWeek) | يضيف نسخة WorkWeek إلى كائن المجموعة هذا. |
| [GetEnumerator](../../aspose.tasks/workweekcollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [ToList](../../aspose.tasks/workweekcollection/tolist/)() | يحوّل كائن `WorkWeekCollection` إلى قائمة من كائنات [`WorkWeek`](../workweek/). |

## الأمثلة

يوضح كيفية إنشاء أسبوع عمل مخصص لتقويم.

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Standard");
Calendar.MakeStandardCalendar(calendar);

var item = new WorkWeek();
item.Name = "My Work Week";
item.FromDate = new DateTime(2020, 4, 13, 8, 0, 0);
item.ToDate = new DateTime(2020, 4, 17, 17, 0, 0);
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
item.WeekDays.Add(new WeekDay(DayType.Saturday));
item.WeekDays.Add(new WeekDay(DayType.Sunday));
calendar.WorkWeeks.Add(item);

Console.WriteLine("Work Weeks Count: " + calendar.WorkWeeks.Count);
foreach (var workWeek in calendar.WorkWeeks)
{
    // اعرض اسم أسبوع العمل، اسم التقويم الأب، وتواريخ البداية والنهاية
    Console.WriteLine("Name: " + workWeek.Name);
    Console.WriteLine("Parent calendar name: " + calendar.Name);
    Console.WriteLine("From Date: " + workWeek.FromDate);
    Console.WriteLine("To Date: " + workWeek.ToDate);
    Console.WriteLine();

    // هذه البيانات تتعلق بالكامل بزر \"Details.\" يمكنك تعيين أوقات عمل خاصة ليوم أسبوع خاص أو حتى جعله غير عامل
    List<WeekDay> weekDays = workWeek.WeekDays.ToList();
    foreach (var day in weekDays)
    {
        Console.WriteLine(day.DayType.ToString());

        // يمكنك أيضًا التنقل عبر أوقات العمل وعرضها
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }

    Console.WriteLine();
}
```

### انظر أيضًا

* class [WorkWeek](../workweek/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


