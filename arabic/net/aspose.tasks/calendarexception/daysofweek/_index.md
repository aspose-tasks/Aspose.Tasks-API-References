---
title: "CalendarException.DaysOfWeek"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية CalendarException. يحصل على DayTypeCollection لهذا الكائن. أيام الأسبوع التي يكون فيها الاستثناء صالحًا"
type: docs
weight: 20
url: /ar/net/aspose.tasks/calendarexception/daysofweek/
---
## CalendarException.DaysOfWeek property

يحصل على DayTypeCollection لهذا الكائن. أيام الأسبوع التي يكون فيها الاستثناء صالحًا.

```csharp
public DayTypeCollection DaysOfWeek { get; }
```

## الأمثلة

يوضح كيفية تعريف استثناء التقويم حسب يوم الأسبوع.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// إنشاء تقويم
var calendar = project.Calendars.Add("Calendar1");

// إنشاء استثناء تقويم لكل يوم جمعة
var exception = new CalendarException();
exception.Type = CalendarExceptionType.Weekly;
exception.FromDate = new DateTime(2020, 4, 6);
exception.ToDate = new DateTime(2020, 4, 12);
exception.DaysOfWeek.Add(DayType.Friday);

// تحقق من أن الجمعة استثنائية
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2020, 4, 10)));

// أضف الاستثناء إلى التقويم
calendar.Exceptions.Add(exception);
```

### انظر أيضًا

* class [DayTypeCollection](../../daytypecollection/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


