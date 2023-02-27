---
title: Class Calendar
second_title: Aspose.Tasks لمرجع .NET API
description: Aspose.Tasks.Calendar فصل. يمثل التقويم المستخدم في مشروع .
type: docs
weight: 230
url: /ar/net/aspose.tasks/calendar/
---
## Calendar class

يمثل التقويم المستخدم في مشروع .

```csharp
public class Calendar
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar/) { get; set; } | الحصول على أو تعيين التقويم الأساسي الذي يعتمد عليه هذا التقويم. ينطبق فقط إذا لم يكن التقويم تقويمًا أساسيًا . |
| [Exceptions](../../aspose.tasks/calendar/exceptions/) { get; } | الحصول على كائن CalendarExceptionCollection . مجموعة الاستثناءات المرتبطة بالتقويم. |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar/) { get; } | يحصل على قيمة تشير إلى ما إذا كان التقويم تقويمًا أساسيًا . |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar/) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان التقويم تقويمًا أساسيًا . |
| [Name](../../aspose.tasks/calendar/name/) { get; set; } | الحصول على أو تحديد اسم التقويم . |
| [Uid](../../aspose.tasks/calendar/uid/) { get; set; } | الحصول على أو تحديد المعرف الفريد للتقويم. |
| [WeekDays](../../aspose.tasks/calendar/weekdays/) { get; } | الحصول على مجموعة أيام الأسبوع لهذا التقويم . مجموعة أيام الأسبوع التي تحدد التقويم. |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks/) { get; } | Gets WorkWeekCollections object. مجموعة أسابيع العمل المرتبطة بالتقويم. |

## طُرق

| اسم | وصف |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar/)(Calendar) | جعل التقويم المحدد 24 ساعة. تقويم 24 ساعة هو تقويم يعمل فيه كل يوم من أيام الأسبوع بساعات عمل على مدار الساعة . |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar/)(Calendar) | إنشاء تقويم معين كتقويم نوبة ليلية . |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar/)(Calendar) | إنشاء تقويم قياسي افتراضي . |
| [Delete](../../aspose.tasks/calendar/delete/)() | إزالة التقويم من المشروع . |
| override [Equals](../../aspose.tasks/calendar/equals/)(object) | إرجاع قيمة تشير إلى ما إذا كان هذا المثيل يساوي كائنًا محددًا. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | حساب التاريخ الذي يمر فيه المقدار المحدد من وقت العمل وفقًا للتقويم. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | حساب التاريخ الذي يمر فيه المقدار المحدد من وقت العمل وفقًا للتقويم. |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode/)() | إرجاع رمز تجزئة لمثيل الفئة. |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart/)(DateTime) | يبدأ حساب يوم العمل التالي من التاريخ. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend/)(DateTime) | حساب نهاية تاريخ العمل السابق من التاريخ المحدد. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | إرجاع تاريخ البدء بناءً على تاريخ الانتهاء والمدة المحددين. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | إرجاع تاريخ البدء بناءً على تاريخ الانتهاء والمدة المحددين. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | حساب تاريخ انتهاء المهمة ووقتها من تاريخ البدء والأجزاء المنقسمة والمدة. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours_1)(DateTime) | إرجاع مقدار ساعات العمل في التاريخ. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | إرجاع ساعات العمل للتواريخ المحددة. |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes/)(DateTime) | عوائد[`WorkingTimeCollection`](../workingtimecollection/) من أوقات العمل في التاريخ المحدد. |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking/)(DateTime) | لتحديد ما إذا كان اليوم هو يوم عمل. |

### ملاحظات

يتم استخدام التقويمات لتحديد أوقات العمل وأوقات غير العمل القياسية. يجب أن يكون للمشروعات تقويم أساسي واحد. يمكن أن تحتوي المهام والموارد على التقويمات غير الأساسية الخاصة بها والتي تستند إلى تقويم أساسي.

### أمثلة

كيفية إنشاء تقويم بسيط من البداية .

```csharp
[C#]
// إنشاء تقويم فارغ
Calendar calendar = new Calendar("New calendar");
// يضيف أيام العمل الافتراضية (8 ساعات عمل من 9:00 إلى 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// إنشاء يوم عمل جديد
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// يعين وقت العمل. فقط جزء الوقت من DateTime مهم
    WorkingTime wt1 = new WorkingTime();
    wt1.FromTime = new DateTime(1, 1, 1, 6, 0, 0, 0);
    wt1.ToTime = new DateTime(1, 1, 1, 12, 0, 0, 0);
    WorkingTime wt2 = new WorkingTime();
    wt2.FromTime = new DateTime(1, 1, 1, 14, 0, 0, 0);
    wt2.ToTime = new DateTime(1, 1, 1, 18, 0, 0, 0);
    myWeekDay.WorkingTimes.Add(wt1);
    myWeekDay.WorkingTimes.Add(wt2);
    myWeekDay.DayWorking = true;
calendar.Days.Add(myWeekDay);
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
// يضيف عطلة نهاية الأسبوع
calendar.Days.Add(new WeekDay(DayType.Saturday));
calendar.Days.Add(new WeekDay(DayType.Sunday));
```

```csharp
[VB]
' إنشاء تقويم فارغ
Dim calendar As Calendar =  New Calendar("New calendar")
' إضافة أيام عمل افتراضية (8 ساعات عمل من 9:00 إلى 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
' إنشاء يوم عمل جديد
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
' يحدد وقت العمل. فقط جزء الوقت من DateTime مهم
    Dim wt1 As WorkingTime =  New WorkingTime()
    wt1.FromTime = New DateTime(1, 1, 1, 6, 0, 0, 0)
    wt1.ToTime = New DateTime(1, 1, 1, 12, 0, 0, 0)
    Dim wt2 As WorkingTime =  New WorkingTime()
    wt2.FromTime = New DateTime(1, 1, 1, 14, 0, 0, 0)
    wt2.ToTime = New DateTime(1, 1, 1, 18, 0, 0, 0)
    myWeekDay.WorkingTimes.Add(wt1)
    myWeekDay.WorkingTimes.Add(wt2)
    myWeekDay.DayWorking = True
calendar.Days.Add(myWeekDay)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday))
' يضيف عطلة نهاية الأسبوع
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

### أنظر أيضا

* مساحة الاسم [Aspose.Tasks](../../aspose.tasks/)
* المجسم [Aspose.Tasks](../../)


