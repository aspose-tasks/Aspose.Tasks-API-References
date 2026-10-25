---
title: "CalendarException.WorkingTimes"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية CalendarException. تحصل أو تعيين كائن WorkingTimeCollection. مجموعة أوقات العمل التي تحدد الوقت العامل في أيام الأسبوع. يجب أن يكون هناك وقت عمل واحد على الأقل ولا يمكن أن يكون أكثر من خمسة."
type: docs
weight: 160
url: /ar/net/aspose.tasks/calendarexception/workingtimes/
---
## CalendarException.WorkingTimes property

يحصل أو يضبط كائن WorkingTimeCollection. مجموعة أوقات العمل التي تحدد الوقت العامل في أيام الأسبوع. يجب أن يكون هناك وقت عمل واحد على الأقل، ولا يمكن أن يكون أكثر من خمسة.

```csharp
public WorkingTimeCollection WorkingTimes { get; set; }
```

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

* class [WorkingTimeCollection](../../workingtimecollection/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


