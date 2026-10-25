---
title: "WeekDay.SetDefaultWorkingTime"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة WeekDay. تعين فترات زمنية افتراضية لليوم الأسبوعي المحدد"
type: docs
weight: 130
url: /ar/net/aspose.tasks/weekday/setdefaultworkingtime/
---
## WeekDay.SetDefaultWorkingTime method

يضبط فترات الوقت الافتراضية ليوم الأسبوع المحدد.

```csharp
public static void SetDefaultWorkingTime(WeekDay day)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| يوم | WeekDay | يوم الأسبوع لتعيين يوم العمل الافتراضي عليه. |

## الأمثلة

يظهر كيفية تعيين وقت عمل افتراضي ليوم.

```csharp
var project = new Project();

// تعريف تقويم
var calendar = project.Calendars.Add("Calendar1");
calendar.WeekDays.Clear();

// إضافة أيام العمل من الاثنين إلى الخميس مع الأوقات الافتراضية
var monday = new WeekDay(DayType.Monday);
WeekDay.SetDefaultWorkingTime(monday);
calendar.WeekDays.Add(monday);
var tuesday = new WeekDay(DayType.Tuesday);
WeekDay.SetDefaultWorkingTime(tuesday);
calendar.WeekDays.Add(tuesday);
var wednesday = new WeekDay(DayType.Wednesday);
WeekDay.SetDefaultWorkingTime(wednesday);
calendar.WeekDays.Add(wednesday);
var thursday = new WeekDay(DayType.Thursday);
WeekDay.SetDefaultWorkingTime(thursday);
calendar.WeekDays.Add(thursday);
var friday = new WeekDay(DayType.Friday);
WeekDay.SetDefaultWorkingTime(friday);
calendar.WeekDays.Add(friday);

var saturday = new WeekDay(DayType.Saturday);
saturday.DayWorking = false;
calendar.WeekDays.Add(saturday);
var sunday = new WeekDay(DayType.Sunday);
sunday.DayWorking = false;
calendar.WeekDays.Add(sunday);

// لنطبع جميع أوقات العمل
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine("Day Type: " + day.DayType); 
    Console.WriteLine("Is working day: " + day.DayWorking); 
    Console.WriteLine("Working Time (Hours): " + day.GetWorkingTime().TotalHours);
    Console.WriteLine();
}
```

### انظر أيضًا

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


