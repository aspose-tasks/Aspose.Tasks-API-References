---
title: "الفئة WeekDay"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.WeekDay. تمثل يوماً من أيام الأسبوع إما يحدد أيامًا عادية من الأسبوع أو أيام استثنائية في تقويم."
type: docs
weight: 3540
url: /ar/net/aspose.tasks/weekday/
---
## WeekDay class

يمثل يومًا من أيام الأسبوع يحدد إما أيامًا عادية في الأسبوع أو أيام استثنائية في التقويم.

```csharp
public class WeekDay
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [WeekDay](weekday/#constructor)() | ينشئ مثيلاً جديدًا للفئة `WeekDay`. |
| [WeekDay](weekday/#constructor_1)(DayType) | ينشئ مثيلاً جديدًا للفئة `WeekDay` بنوع اليوم المحدد. |
| [WeekDay](weekday/#constructor_3)(DayType, IEnumerable&lt;WorkingTime&gt;) | ينشئ مثيلاً جديدًا للفئة `WeekDay` بنوع اليوم المحدد وقائمة فترات وقت العمل. |
| [WeekDay](weekday/#constructor_2)(DayType, params WorkingTime[]) | ينشئ مثيلاً جديدًا للفئة `WeekDay` بنوع اليوم المحدد وفترات وقت العمل. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [DayType](../../aspose.tasks/weekday/daytype/) { get; } | يحصل على نوع اليوم. |
| [DayWorking](../../aspose.tasks/weekday/dayworking/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان التاريخ أو نوع اليوم المحدد يعمل. |
| [FromDate](../../aspose.tasks/weekday/fromdate/) { get; set; } | يحصل أو يضبط بداية وقت الاستثناء. |
| [ToDate](../../aspose.tasks/weekday/todate/) { get; set; } | يحصل أو يضبط نهاية وقت الاستثناء. |
| [WorkingTimes](../../aspose.tasks/weekday/workingtimes/) { get; } | يحصل على WorkingTimeCollection لهذا المثيل WeekDay. مجموعة أوقات العمل التي تحدد الوقت العامل في يوم الأسبوع. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [CreateDefaultWorkingDay](../../aspose.tasks/weekday/createdefaultworkingday/)(DayType) | ينشئ يوم عمل افتراضي. |
| [Clone](../../aspose.tasks/weekday/clone/)() | يعيد نسخة عميقة من يوم الأسبوع. |
| override [Equals](../../aspose.tasks/weekday/equals/)(object) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| override [GetHashCode](../../aspose.tasks/weekday/gethashcode/)() | يعيد قيمة رمز تجزئة للمثيل من الفئة `WeekDay`. |
| [GetWorkingTime](../../aspose.tasks/weekday/getworkingtime/)() | يعيد وقت العمل ليوم أسبوع. |
| static [CastToDayType](../../aspose.tasks/weekday/casttodaytype/)(DayOfWeek) | يحوّل DayOfWeek الخاص بـ .Net إلى [`DayType`](./daytype/). |
| static [SetDefaultWorkingTime](../../aspose.tasks/weekday/setdefaultworkingtime/)(WeekDay) | يضبط فترات الوقت الافتراضية ليوم الأسبوع المحدد. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


