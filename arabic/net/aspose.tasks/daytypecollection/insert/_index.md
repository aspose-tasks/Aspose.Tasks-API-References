---
title: "DayTypeCollection.Insert"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة DayTypeCollection. تُدرج العنصر المحدد في الفهرس المحدد"
type: docs
weight: 100
url: /ar/net/aspose.tasks/daytypecollection/insert/
---
## DayTypeCollection.Insert method

يدرج العنصر المحدد في الفهرس المحدد.

```csharp
public void Insert(int index, DayType item)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| الفهرس | Int32 | الفهرس الصفري المحدد الذي يجب إدراج العنصر فيه. |
| العنصر | DayType | العنصر المحدد لإدراجه في هذه المجموعة. |

## الأمثلة

يوضح كيفية استخدام مجموعة أيام الأسبوع لتحديد استثناء تقويم أسبوعي.

```csharp
var project = new Project(DataDir + "WeeklyDayTypeException.mpp");
var calendar = project.Calendars.GetByUid(1);

foreach (var calendarException in calendar.Exceptions)
{
    Console.WriteLine("Exception Name: " + calendarException.Name);
    Console.WriteLine("Days of week count: " + calendarException.DaysOfWeek.Count);
    foreach (var dayType in calendarException.DaysOfWeek)
    {
        Console.WriteLine("Day type: " + dayType);
    }

    Console.WriteLine();
}

var exc1 = calendar.Exceptions.ToList()[0];
if (!exc1.DaysOfWeek.IsReadOnly && exc1.DaysOfWeek.IndexOf(DayType.Monday) < 0)
{
    exc1.DaysOfWeek.Insert(0, DayType.Wednesday);
}

var exc2 = calendar.Exceptions.ToList()[1];
if (exc2.DaysOfWeek.Contains(DayType.Sunday))
{
    // حذف نوع يوم من \"Exception 2\" حسب نوع اليوم
    exc2.DaysOfWeek.Remove(DayType.Sunday);
}

// حذف نوع يوم من \"Exception 2\" حسب الفهرس
Console.WriteLine("Remove " + exc2.DaysOfWeek[0] + " day type from exception by index...");
exc2.DaysOfWeek.RemoveAt(0);

// تغيير الاستثناءات (لا توجد استثناءات في بيانات المشروع الأولية)
var exc4 = new CalendarException
               {
                   Name = "Weekly Exception 2",
                   FromDate = new DateTime(2020, 4, 13),
                   ToDate = new DateTime(2020, 4, 18),
                   Occurrences = 3,
                   Type = CalendarExceptionType.Weekly
               };
exc4.DaysOfWeek.Add(DayType.Monday);
exc4.DaysOfWeek.Add(DayType.Thursday);

calendar.Exceptions.Add(exc4);

var exc3 = calendar.Exceptions.ToList()[2];

// إزالة جميع أيام الأسبوع لـ \"Exception 3\"
exc3.DaysOfWeek.Clear();

var dayTypes = new DayType[exc4.DaysOfWeek.Count];
exc4.DaysOfWeek.CopyTo(dayTypes, 0);

foreach (var dayType in dayTypes)
{
    exc3.DaysOfWeek.Add(dayType);
}

Console.WriteLine("Days of week for exception: " + exc3.Name);
foreach (var dayType in exc3.DaysOfWeek)
{
    Console.WriteLine("Day type: " + dayType);
}
```

### انظر أيضًا

* enum [DayType](../../daytype/)
* class [DayTypeCollection](../)
* namespace [Aspose.Tasks](../../daytypecollection/)
* assembly [Aspose.Tasks](../../../)


