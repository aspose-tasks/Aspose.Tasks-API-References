---
title: "الفئة Calendar"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Calendar. تمثّل تقويمًا يُستخدم في مشروع"
type: docs
weight: 230
url: /ar/net/aspose.tasks/calendar/
---
## Calendar class

يمثل تقويمًا يُستخدم في مشروع.

```csharp
public class Calendar : ICalendar
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar/) { get; set; } | يحصل أو يعيّن التقويم الأساسي الذي يعتمد عليه هذا التقويم. ينطبق فقط إذا لم يكن التقويم تقويمًا أساسيًا. |
| [Exceptions](../../aspose.tasks/calendar/exceptions/) { get; } | يحصل على كائن CalendarExceptionCollection. مجموعة الاستثناءات المرتبطة بالتقويم. |
| [Guid](../../aspose.tasks/calendar/guid/) { get; } | يحصل على معرف الـ Guid الخاص بالتقويم. |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar/) { get; } | يحصل على قيمة تشير إلى ما إذا كان التقويم تقويمًا أساسيًا. |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان التقويم تقويمًا خط أساس. |
| [Name](../../aspose.tasks/calendar/name/) { get; set; } | يحصل أو يعيّن اسم التقويم. |
| [PrimaveraProperties](../../aspose.tasks/calendar/primaveraproperties/) { get; } | يحصل على كائن يحتوي على خصائص خاصة بـ Primavera لتقويم تم قراءته من صيغ Primavera. |
| [Uid](../../aspose.tasks/calendar/uid/) { get; set; } | يحصل أو يعيّن المعرف الفريد للتقويم. |
| [WeekDays](../../aspose.tasks/calendar/weekdays/) { get; } | يحصل على WeekDaysCollection لهذا التقويم. مجموعة أيام الأسبوع التي تُعرّف التقويم. |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks/) { get; } | يحصل على كائن WorkWeekCollections. مجموعة أسابيع العمل المرتبطة بالتقويم. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar/)(Calendar) | يجعل تقويمًا معينًا تقويمًا 24 ساعة. تقويم 24 ساعة هو تقويم يعمل فيه كل يوم من الأسبوع بساعات عمل مستمرة على مدار الساعة. |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar/)(Calendar) | يجعل التقويم المحدد تقويمًا للوردية الليلية. |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar/)(Calendar) | ينشئ تقويمًا قياسيًا افتراضيًا. |
| [Delete](../../aspose.tasks/calendar/delete/)() | يزيل التقويم من المشروع. |
| override [Equals](../../aspose.tasks/calendar/equals/)(object) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | يحسب التاريخ الذي سينقضي فيه مقدار وقت العمل المحدد وفقًا للتقويم. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | يحسب التاريخ الذي سينقضي فيه مقدار وقت العمل المحدد وفقًا للتقويم. |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode/)() | يعيد رمز تجزئة (hash) لنسخة الفئة. |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart/)(DateTime) | يحسب بداية يوم العمل التالي للتاريخ المحدد. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend/)(DateTime) | يحسب نهاية تاريخ العمل السابق من التاريخ المحدد. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | يرجع تاريخ البدء بناءً على تاريخ الانتهاء المحدد والمدة. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | يرجع تاريخ البدء بناءً على تاريخ الانتهاء المحدد والمدة. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | يحسب تاريخ ووقت انتهاء المهمة من تاريخ بدايتها، الأجزاء المقسمة ومدة العمل. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours_1)(DateTime) | يرجع مقدار ساعات العمل في التاريخ المحدد. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | إرجاع وحدة العمل - البداية، النهاية ومدة ساعات العمل للفترة الزمنية المحددة. |
| [GetWorkingHoursTimeSpan](../../aspose.tasks/calendar/getworkinghourstimespan/)(DateTime, DateTime) | يرجع مقدار ساعات العمل بين التواريخ المحددة. |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes/)(DateTime) | يرجع [`WorkingTimeCollection`](../workingtimecollection/) لأوقات العمل للتاريخ المحدد. |
| [GetWorkStart](../../aspose.tasks/calendar/getworkstart/)(DateTime) | يحسب بداية وقت العمل التالي بدءًا من التاريخ والوقت المحددين. |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking/)(DateTime) | يحدد ما إذا كان اليوم المحدد يوم عمل وفقًا للتقويم. |
| virtual [IsEmpty](../../aspose.tasks/calendar/isempty/)() | يرجع ما إذا كان التقويم لا يحتوي على ساعات عمل معرفة. |
| static [GetIntersectionCalendar](../../aspose.tasks/calendar/getintersectioncalendar/)(Calendar, Calendar) | يحصل على نسخة [`ICalendar`](../icalendar/) التي يمكن استخدامها لإجراء حسابات على تقاطع جداول العمل لتقويمين. |

## ملاحظات

يُستخدم التقويم لتعريف أوقات العمل القياسية وغير القياسية. يجب أن يكون للمشروعات تقويم أساسي واحد. يمكن للمهام والموارد أن تمتلك تقويمات غير أساسية خاصة بها تعتمد على التقويم الأساسي.

## الأمثلة

كيفية إنشاء تقويم بسيط من الصفر.

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
// يضبط وقت العمل. الجزء الزمني فقط من DateTime هو المهم
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
' create empty calendar
Dim calendar As Calendar =  New Calendar("New calendar")
' adds default working days (8 working hours from 9:00 to 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
' create new new working day
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
' Sets working time. Only time part of DateTime is important
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
' adds weekend
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

يظهر كيفية تعريف تقويم جديد، إضافة أيام الأسبوع إليه وتعريف أوقات العمل للأيام.

```csharp
var project = new Project();

// تعريف تقويم
var calendar = project.Calendars.Add("Calendar1");

// إضافة أيام العمل من الاثنين إلى الخميس مع الأوقات الافتراضية
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// تعيين الجمعة كيوم عمل قصير
var weekDay = new WeekDay(DayType.Friday);

// يضبط وقت العمل. الجزء الزمني فقط من DateTime هو المهم
var workingTime = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 16);
weekDay.WorkingTimes.Add(workingTime);
weekDay.WorkingTimes.Add(workingTime2);
weekDay.DayWorking = true;
calendar.WeekDays.Add(weekDay);

// العمل مع المشروع...
```

### انظر أيضًا

* interface [ICalendar](../icalendar/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


