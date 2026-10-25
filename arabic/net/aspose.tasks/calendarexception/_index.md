---
title: "الفئة CalendarException"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.CalendarException. تمثل فترات زمنية استثنائية في التقويم"
type: docs
weight: 250
url: /ar/net/aspose.tasks/calendarexception/
---
## CalendarException class

يمثل فترات زمنية استثنائية في تقويم.

```csharp
public sealed class CalendarException
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [CalendarException](calendarexception/)() | ينشئ مثيلاً جديداً من الفئة `CalendarException`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [DaysOfWeek](../../aspose.tasks/calendarexception/daysofweek/) { get; } | يحصل على DayTypeCollection لهذا الكائن. أيام الأسبوع التي يكون فيها الاستثناء صالحًا. |
| [DayWorking](../../aspose.tasks/calendarexception/dayworking/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان التاريخ أو نوع اليوم المحدد يعمل. |
| [EnteredByOccurrences](../../aspose.tasks/calendarexception/enteredbyoccurrences/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان نطاق التكرار معرفًا بإدخال عدد مرات التكرار. القيمة False تعني أن نطاق التكرار معرف بإدخال تاريخ الانتهاء. |
| [FromDate](../../aspose.tasks/calendarexception/fromdate/) { get; set; } | يحصل أو يضبط بداية وقت الاستثناء. |
| [Month](../../aspose.tasks/calendarexception/month/) { get; set; } | يحصل أو يضبط الشهر الذي يُجدول فيه تكرار الاستثناء. |
| [MonthDay](../../aspose.tasks/calendarexception/monthday/) { get; set; } | يحصل أو يضبط يوم الشهر الذي يُجدول فيه تكرار الاستثناء. |
| [MonthItem](../../aspose.tasks/calendarexception/monthitem/) { get; set; } | يحصل أو يضبط عنصر الشهر الذي يُجدول فيه تكرار الاستثناء. |
| [MonthPosition](../../aspose.tasks/calendarexception/monthposition/) { get; set; } | يحصل أو يضبط موضع عنصر الشهر داخل الشهر. |
| [Name](../../aspose.tasks/calendarexception/name/) { get; set; } | يحصل أو يضبط اسم الاستثناء. |
| [Occurrences](../../aspose.tasks/calendarexception/occurrences/) { get; set; } | يحصل أو يضبط عدد مرات التكرار التي يكون فيها استثناء التقويم صالحًا. |
| [ParentCalendar](../../aspose.tasks/calendarexception/parentcalendar/) { get; } | يحصل على التقويم الأب لهذا الكائن. |
| [Period](../../aspose.tasks/calendarexception/period/) { get; set; } | يحصل أو يضبط فترة تكرار الاستثناء. |
| [ToDate](../../aspose.tasks/calendarexception/todate/) { get; set; } | يحصل أو يضبط نهاية وقت الاستثناء. |
| [Type](../../aspose.tasks/calendarexception/type/) { get; set; } | يحصل أو يضبط نوع الاستثناء. |
| [WorkingTimes](../../aspose.tasks/calendarexception/workingtimes/) { get; set; } | يحصل أو يضبط كائن WorkingTimeCollection. مجموعة أوقات العمل التي تحدد الوقت العامل في أيام الأسبوع. يجب أن يكون هناك وقت عمل واحد على الأقل، ولا يمكن أن يكون أكثر من خمسة. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [CheckException](../../aspose.tasks/calendarexception/checkexception/)(DateTime) | يعيد true إذا كان المثيل المحدد للهيكل DateTime هو يوم الاستثناء. |
| [Delete](../../aspose.tasks/calendarexception/delete/)() | يحذف مثيل Exception من كائن التقويم الأب CalendarExceptionCollection. |
| [GetExceptionDates](../../aspose.tasks/calendarexception/getexceptiondates/)() | يعيد التواريخ التي ينطبق عليها استثناء التقويم. |
| [GetWorkingTime](../../aspose.tasks/calendarexception/getworkingtime/)() | يعيد وقت العمل لاستثناء التقويم. |

## الأمثلة

يظهر كيفية إضافة/إزالة استثناءات التقويم.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// إنشاء تقويم
var calendar = project.Calendars.Add("Calendar1");

// إنشاء استثناء أيام الأسبوع لعطلة
var exception = new CalendarException();
exception.Name = "New Calendar Exception";
exception.EnteredByOccurrences = false;
exception.FromDate = new DateTime(2009, 12, 24, 0, 0, 0);
exception.ToDate = new DateTime(2009, 12, 31, 23, 59, 0);
exception.Type = CalendarExceptionType.Daily;
exception.Month = Month.December;

exception.DayWorking = false;

// تحقق من أن التاريخ استثنائي
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2009, 12, 26, 8, 0, 0)));

calendar.Exceptions.Add(exception);

// إزالة استثناء
var cal = project.Calendars.ToList()[0];
if (cal.Exceptions.Count > 1)
{
    var excToRemove = cal.Exceptions[0];
    cal.Exceptions.Remove(excToRemove);
}

// إضافة استثناء
var exception2 = new CalendarException();
exception2.FromDate = new System.DateTime(2009, 1, 1);
exception2.ToDate = new System.DateTime(2009, 1, 3);
cal.Exceptions.Add(exception2);

// طباعة الاستثناءات
foreach (var exc in cal.Exceptions)
{
    Console.WriteLine("Name: " + exc.Name);
    Console.WriteLine("From: " + exc.FromDate.ToShortDateString());
    Console.WriteLine("To: " + exc.ToDate.ToShortDateString());
}
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


