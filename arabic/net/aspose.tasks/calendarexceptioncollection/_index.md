---
title: "الفئة CalendarExceptionCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.CalendarExceptionCollection. تمثل مجموعة من كائنات CalendarException"
type: docs
weight: 260
url: /ar/net/aspose.tasks/calendarexceptioncollection/
---
## CalendarExceptionCollection class

تمثل مجموعة من كائنات [`CalendarException`](../calendarexception/).

```csharp
public class CalendarExceptionCollection : IList<CalendarException>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/calendarexceptioncollection/count/) { get; } | يحصل على عدد الكائنات المحتواة في كائن `CalendarExceptionCollection` هذا. |
| [Item](../../aspose.tasks/calendarexceptioncollection/item/) { get; set; } | يرجع العنصر عند الفهرس المحدد. |
| [ParentCalendar](../../aspose.tasks/calendarexceptioncollection/parentcalendar/) { get; } | يحصل على التقويم الأب لهذا الكائن. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks/calendarexceptioncollection/add/)(CalendarException) | يضيف كائن CalendarException إلى كائن التجميع هذا. |
| [AddRange](../../aspose.tasks/calendarexceptioncollection/addrange/)(IEnumerable&lt;CalendarException&gt;) | يضيف نطاقًا من الاستثناءات إلى القائمة الداخلية. |
| [Clear](../../aspose.tasks/calendarexceptioncollection/clear/)() | يزيل جميع العناصر من `CalendarExceptionCollection`. |
| [GetEnumerator](../../aspose.tasks/calendarexceptioncollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [Remove](../../aspose.tasks/calendarexceptioncollection/remove/)(CalendarException) | يزيل نسخة [`CalendarException`](../calendarexception/) من هذا التجميع. |
| [ToList](../../aspose.tasks/calendarexceptioncollection/tolist/)() | يحول كائن CalendarExceptionCollection إلى قائمة من كائنات [`CalendarException`](../calendarexception/). |

## الأمثلة

يوضح كيفية استخدام مجموعة استثناءات التقويم لتعريف استثناءات التقويم.

```csharp
var project = new Project(DataDir + "project_update_test.mpp");
var calendar = project.Calendars.GetByUid(3);

calendar.Exceptions.Clear();
Calendar.MakeStandardCalendar(calendar);

var exception = new CalendarException();
exception.FromDate = new DateTime(2020, 3, 30, 8, 0, 0);
exception.ToDate = new DateTime(2020, 4, 3, 17, 0, 0);
exception.DayWorking = true;
exception.Name = "Exception 1";

var wt1 = new WorkingTime(9, 13);
var wt2 = new WorkingTime(14, 19);

exception.WorkingTimes.Add(wt1);
exception.WorkingTimes.Add(wt2);
calendar.Exceptions.Add(exception);

var nonWorkingExceptions = new CalendarException[2];
nonWorkingExceptions[0] = new CalendarException();
nonWorkingExceptions[0].FromDate = new DateTime(2020, 4, 13, 8, 0, 0);
nonWorkingExceptions[0].ToDate = new DateTime(2020, 4, 18, 17, 0, 0);
nonWorkingExceptions[0].DayWorking = false;
nonWorkingExceptions[0].Name = "Exception 2";
nonWorkingExceptions[1] = new CalendarException();
nonWorkingExceptions[1].FromDate = new DateTime(2020, 4, 6, 8, 0, 0);
nonWorkingExceptions[1].ToDate = new DateTime(2020, 4, 10, 17, 0, 0);
nonWorkingExceptions[1].DayWorking = false;
nonWorkingExceptions[1].Name = "Exception 3";
calendar.Exceptions.AddRange(nonWorkingExceptions);

Console.WriteLine("Exceptions of calendar {0}: ", calendar.Exceptions.ParentCalendar.Name);
Console.WriteLine("Exceptions count: {0}", calendar.Exceptions.Count);
Console.WriteLine();
foreach (var calendarException in calendar.Exceptions)
{
    Console.WriteLine("Name: " + calendarException.Name);
    Console.WriteLine("From Date: " + calendarException.FromDate);
    Console.WriteLine("To Date: " + calendarException.ToDate);
    Console.WriteLine("Is day working: " + calendarException.DayWorking);
    Console.WriteLine();
}

// إزالة جميع الاستثناءات
Console.WriteLine("Remove calendar exceptions...");
List<CalendarException> exceptions = calendar.Exceptions.ToList();
foreach (var calendarException in exceptions)
{
    Console.WriteLine("Remove exception: " + calendarException.Name);
    Console.WriteLine();
    calendar.Exceptions.Remove(calendarException);
}
```

### انظر أيضًا

* class [CalendarException](../calendarexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


