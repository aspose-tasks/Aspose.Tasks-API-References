---
title: "الفئة WeekDayCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.WeekDayCollection. تمثّل مجموعة من كائنات WeekDay"
type: docs
weight: 3550
url: /ar/net/aspose.tasks/weekdaycollection/
---
## WeekDayCollection class

تمثّل مجموعة من كائنات [`WeekDay`](../weekday/).

```csharp
public class WeekDayCollection : IList<WeekDay>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/weekdaycollection/count/) { get; } | يحصل على عدد الكائنات الموجودة في كائن `WeekDayCollection` هذا. |
| [Item](../../aspose.tasks/weekdaycollection/item/) { get; set; } | يحصل أو يعيّن قيمة العنصر في الفهرس المحدد. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks/weekdaycollection/add/)(WeekDay) | يضيف نسخة من [`WeekDay`](../weekday/) إلى هذا الكائن. |
| [Clear](../../aspose.tasks/weekdaycollection/clear/)() | امسح كائن WeekDayCollection. |
| [Contains](../../aspose.tasks/weekdaycollection/contains/)(WeekDay) | يتحقق مما إذا كانت المجموعة تحتوي على [`WeekDay`](../weekday/).specified. |
| [CopyTo](../../aspose.tasks/weekdaycollection/copyto/)(WeekDay[], int) | ينسخ محتوى المجموعة إلى مصفوفة في الفهرس المحدد. |
| [GetEnumerator](../../aspose.tasks/weekdaycollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [IndexOf](../../aspose.tasks/weekdaycollection/indexof/)(WeekDay) | يعيد الفهرس للـ [`WeekDay`](../weekday/) المحدد. |
| [Insert](../../aspose.tasks/weekdaycollection/insert/)(int, WeekDay) | يدرج [`WeekDay`](../weekday/) في الفهرس المحدد. |
| [Remove](../../aspose.tasks/weekdaycollection/remove/)(WeekDay) | يزيل [`WeekDay`](../weekday/) المحدد، إن وجد. |
| [RemoveAt](../../aspose.tasks/weekdaycollection/removeat/)(int) | يزيل عنصرًا في الفهرس المحدد. |
| [ToList](../../aspose.tasks/weekdaycollection/tolist/)() | يحوّل كائن WeekDayCollection إلى قائمة من كائنات [`WeekDay`](../weekday/). |

## الأمثلة

يظهر كيفية التعامل مع مجموعات أيام الأسبوع.

```csharp
var project = new Project();
var calendar = project.Calendars.GetByName("Standard");

// مسح أيام الأسبوع
calendar.WeekDays.Clear();

calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
var saturday = WeekDay.CreateDefaultWorkingDay(DayType.Saturday);
var sunday = WeekDay.CreateDefaultWorkingDay(DayType.Sunday);

calendar.WeekDays.Add(saturday);
calendar.WeekDays.Add(sunday);

var fridayWorkingTimes = new List<WorkingTime> { new WorkingTime(new DateTime(2020, 4, 13, 8, 0, 0), new DateTime(2020, 4, 13, 12, 0, 0)) };

var friday = new WeekDay(DayType.Friday, fridayWorkingTimes);
if (calendar.WeekDays.Contains(friday))
{
    calendar.WeekDays.Insert(4, friday);
}

Console.WriteLine("Calendar: " + calendar.Name);
Console.WriteLine("Week days count: " + calendar.WeekDays.Count);
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine(day.DayType);
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine("From: " + workingTime.From);
        Console.WriteLine("To: " + workingTime.To);
        Console.WriteLine();
    }
}

// إزالة يوم السبت من الأسبوع
calendar.WeekDays.RemoveAt(5);

// إزالة يوم الأحد من الأسبوع
if (calendar.WeekDays.IndexOf(saturday) > 0)
{
    calendar.WeekDays.Remove(sunday);
}

Console.WriteLine("Working times after weekend was removed: ");
List<WeekDay> weekDays = calendar.WeekDays.ToList();
foreach (var day in weekDays)
{
    Console.WriteLine(day.DayType);
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine("From: " + workingTime.From);
        Console.WriteLine("To: " + workingTime.To);
        Console.WriteLine();
    }
}

var hour24Calendar = project.Calendars.Add("24 Hours");
Calendar.Make24HourCalendar(hour24Calendar);

// نسخ أيام الأسبوع
var weekDaysArray = new WeekDay[calendar.WeekDays.Count];
calendar.WeekDays.CopyTo(weekDaysArray, 0);

foreach (var weekDay in weekDaysArray)
{
    hour24Calendar.WeekDays.Add(weekDay);
}
```

### انظر أيضًا

* class [WeekDay](../weekday/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


