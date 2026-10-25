---
title: "WeekDay.CreateDefaultWorkingDay"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة WeekDay. تنشئ يوم عمل افتراضي"
type: docs
weight: 20
url: /ar/net/aspose.tasks/weekday/createdefaultworkingday/
---
## WeekDay.CreateDefaultWorkingDay method

ينشئ يوم عمل افتراضي.

```csharp
public static WeekDay CreateDefaultWorkingDay(DayType dayType)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| dayType | DayType | نوع اليوم لإنشاء يوم عمل افتراضي منه. |

### قيمة الإرجاع

يوم عمل افتراضي بأوقات عمل 8-12 و 13-17.

## الأمثلة

يظهر كيفية إنشاء تقويم جديد عن طريق تعريف أيام الأسبوع.

```csharp
var project = new Project();

// تعريف تقويم
var calendar = project.Calendars.Add("Calendar1");

// إضافة أيام العمل من الاثنين إلى الخميس مع الأوقات الافتراضية
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, new WorkingTime(9, 11), new WorkingTime(12, 18)));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));

var exceptionDay = WeekDay.CreateDefaultWorkingDay(DayType.Exception);
exceptionDay.FromDate = new DateTime(2020, 4, 27, 0, 0, 0);
exceptionDay.ToDate = new DateTime(2020, 4, 30, 0, 0, 0);
exceptionDay.DayWorking = false;
calendar.WeekDays.Add(exceptionDay);

// تحقق من تواريخ البداية والنهاية ليوم الاستثناء
Console.WriteLine("The from date is: " + exceptionDay.FromDate);
Console.WriteLine("The to date is: " + exceptionDay.ToDate);
Console.WriteLine();

calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// تعيين الجمعة كيوم عمل قصير

// يضبط وقت العمل. 
var workingTimes = new List<WorkingTime> { new WorkingTime(9, 12), new WorkingTime(13, 16) };

// هناك طريقة لتحويل <see cref="DayOfWeek" /> إلى <see cref="Aspose.Tasks.DayType" />.
var dayType = WeekDay.CastToDayType(DayOfWeek.Friday);

var weekDay = new WeekDay(dayType, workingTimes);
weekDay.DayWorking = true;
Console.WriteLine("The day type is: " + weekDay.DayType);
Console.WriteLine("The from date is: " + weekDay.FromDate);
Console.WriteLine("The to date is: " + weekDay.ToDate);

calendar.WeekDays.Add(weekDay);

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

* enum [DayType](../../daytype/)
* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


