---
title: "الفئة WorkWeek"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.WorkWeek. تمثيل فئة WorkWeek"
type: docs
weight: 3640
url: /ar/net/aspose.tasks/workweek/
---
## WorkWeek class

يمثل فئة WorkWeek

```csharp
public class WorkWeek
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [WorkWeek](workweek/)() | يقوم بتهيئة نسخة جديدة من الفئة `WorkWeek`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [FromDate](../../aspose.tasks/workweek/fromdate/) { get; set; } | يحصل أو يضبط start DateTime لأسبوع العمل |
| [Name](../../aspose.tasks/workweek/name/) { get; set; } | يحصل أو يضبط Name لأسبوع العمل |
| [ToDate](../../aspose.tasks/workweek/todate/) { get; set; } | يحصل أو يضبط Finish DateTime لأسبوع العمل |
| [WeekDays](../../aspose.tasks/workweek/weekdays/) { get; } | يحصل على أيام الأسبوع. |

## الأمثلة

يوضح كيفية قراءة معلومات أسبوع العمل من المشروع.

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

Console.WriteLine("Work Week Number: " + calendar.WeekDays.Count);
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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


