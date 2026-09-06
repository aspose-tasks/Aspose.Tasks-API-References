---
title: "CalendarException.GetWorkingTime"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة CalendarException. تُعيد وقت العمل لاستثناء التقويم"
type: docs
weight: 200
url: /ar/net/aspose.tasks/calendarexception/getworkingtime/
---
## CalendarException.GetWorkingTime method

يعيد وقت العمل لاستثناء التقويم.

```csharp
public TimeSpan GetWorkingTime()
```

### قيمة الإرجاع

تُعيد وقت العمل لهذا الاستثناء في التقويم.

## الأمثلة

يظهر كيفية الحصول على وقت عمل لاستثناء التقويم.

```csharp
var project = new Project(DataDir + "CalendarExceptions.mpp");

var calendar = project.Calendars.ToList()[0];
var exception = calendar.Exceptions[0];

Console.WriteLine("Calendar Name: " + calendar.Name);
Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);
Console.WriteLine("Calendar Exception Name: " + exception.Name);
Console.WriteLine();

var workingTime = exception.GetWorkingTime();
Console.WriteLine("Exception Working Time: " + workingTime);

foreach (var time in exception.WorkingTimes)
{
    Console.WriteLine("Working Time Start: " + time.From);
    Console.WriteLine("Working Time Finish: " + time.To);
}
```

### انظر أيضًا

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


